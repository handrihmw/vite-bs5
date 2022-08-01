<template>
  <div class="sidebar-wrapper active">
    <div class="sidebar-header">
      <div class="d-flex justify-content-between">
        <div class="logo">
          <nuxt-link to="/">
            <img src="~assets/images/logo/nh-dark.svg" alt="Logo" />
          </nuxt-link>
        </div>
        <div class="toggler">
          <a href="#" class="sidebar-hide d-xl-none d-block"
            ><svg
              xmlns="http://www.w3.org/2000/svg"
              width="16"
              height="16"
              fill="currentColor"
              class="bi bi-justify"
              viewBox="0 0 16 16"
            >
              <path
                fill-rule="evenodd"
                d="M2 12.5a.5.5 0 0 1 .5-.5h11a.5.5 0 0 1 0 1h-11a.5.5 0 0 1-.5-.5zm0-3a.5.5 0 0 1 .5-.5h11a.5.5 0 0 1 0 1h-11a.5.5 0 0 1-.5-.5zm0-3a.5.5 0 0 1 .5-.5h11a.5.5 0 0 1 0 1h-11a.5.5 0 0 1-.5-.5zm0-3a.5.5 0 0 1 .5-.5h11a.5.5 0 0 1 0 1h-11a.5.5 0 0 1-.5-.5z"
              /></svg
          ></a>
        </div>
      </div>
    </div>
    <div class="sidebar-menu">
      <ul class="menu">
        <template v-for="item in items" :key="item.key">
          <li class="sidebar-title" v-if="item.isTitle" :key="item.key">
            {{ item.name }}
          </li>
          <li
            class="sidebar-item"
            :class="{
              active: isActive(item.url) || subIsActive(item),
              'has-sub': isHasSub(item),
            }"
            v-else
          >
            <template v-if="isHasSub(item)">
              <a class="sidebar-link">
                <!-- <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="16"
                  height="16"
                  fill="currentColor"
                  class="bi bi-stack"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="m14.12 10.163 1.715.858c.22.11.22.424 0 .534L8.267 15.34a.598.598 0 0 1-.534 0L.165 11.555a.299.299 0 0 1 0-.534l1.716-.858 5.317 2.659c.505.252 1.1.252 1.604 0l5.317-2.66zM7.733.063a.598.598 0 0 1 .534 0l7.568 3.784a.3.3 0 0 1 0 .535L8.267 8.165a.598.598 0 0 1-.534 0L.165 4.382a.299.299 0 0 1 0-.535L7.733.063z"
                  />
                  <path
                    d="m14.12 6.576 1.715.858c.22.11.22.424 0 .534l-7.568 3.784a.598.598 0 0 1-.534 0L.165 7.968a.299.299 0 0 1 0-.534l1.716-.858 5.317 2.659c.505.252 1.1.252 1.604 0l5.317-2.659z"
                  />
                </svg> -->
                <span>{{ item.name }}</span>
              </a>
              <ul class="submenu" :class="{ active: subIsActive(item) }">
                <template v-for="sub in item.submenu" :key="sub.key">
                  <li
                    class="submenu-item"
                    :class="{ active: isActive(sub.url) }"
                  >
                    <nuxt-link :to="sub.url">{{ sub.name }}</nuxt-link>
                  </li>
                </template>
              </ul>
            </template>
            <template v-else>
              <nuxt-link class="sidebar-link" :to="item.url">
                <!-- <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="16"
                  height="16"
                  fill="currentColor"
                  class="bi bi-grid-fill"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="M1 2.5A1.5 1.5 0 0 1 2.5 1h3A1.5 1.5 0 0 1 7 2.5v3A1.5 1.5 0 0 1 5.5 7h-3A1.5 1.5 0 0 1 1 5.5v-3zm8 0A1.5 1.5 0 0 1 10.5 1h3A1.5 1.5 0 0 1 15 2.5v3A1.5 1.5 0 0 1 13.5 7h-3A1.5 1.5 0 0 1 9 5.5v-3zm-8 8A1.5 1.5 0 0 1 2.5 9h3A1.5 1.5 0 0 1 7 10.5v3A1.5 1.5 0 0 1 5.5 15h-3A1.5 1.5 0 0 1 1 13.5v-3zm8 0A1.5 1.5 0 0 1 10.5 9h3a1.5 1.5 0 0 1 1.5 1.5v3a1.5 1.5 0 0 1-1.5 1.5h-3A1.5 1.5 0 0 1 9 13.5v-3z"
                  />
                </svg> -->
                <span>{{ item.name }}</span>
              </nuxt-link>
            </template>
          </li>
        </template>
      </ul>
    </div>
    <button class="sidebar-toggler btn x"><i data-feather="x"></i></button>
  </div>
</template>

<script>
import dataSidebar from "~/store/data/sideBarItems.js";

export default {
  mounted() {
    function slideToggle(t, e, o) {
      0 === t.clientHeight ? j(t, e, o, !0) : j(t, e, o);
    }
    function slideUp(t, e, o) {
      j(t, e, o);
    }
    function slideDown(t, e, o) {
      j(t, e, o, !0);
    }
    function j(t, e, o, i) {
      void 0 === e && (e = 400),
        void 0 === i && (i = !1),
        (t.style.overflow = "hidden"),
        i && (t.style.display = "block");
      var p,
        l = window.getComputedStyle(t),
        n = parseFloat(l.getPropertyValue("height")),
        a = parseFloat(l.getPropertyValue("padding-top")),
        s = parseFloat(l.getPropertyValue("padding-bottom")),
        r = parseFloat(l.getPropertyValue("margin-top")),
        d = parseFloat(l.getPropertyValue("margin-bottom")),
        g = n / e,
        y = a / e,
        m = s / e,
        u = r / e,
        h = d / e;
      window.requestAnimationFrame(function l(x) {
        void 0 === p && (p = x);
        var f = x - p;
        i
          ? ((t.style.height = g * f + "px"),
            (t.style.paddingTop = y * f + "px"),
            (t.style.paddingBottom = m * f + "px"),
            (t.style.marginTop = u * f + "px"),
            (t.style.marginBottom = h * f + "px"))
          : ((t.style.height = n - g * f + "px"),
            (t.style.paddingTop = a - y * f + "px"),
            (t.style.paddingBottom = s - m * f + "px"),
            (t.style.marginTop = r - u * f + "px"),
            (t.style.marginBottom = d - h * f + "px")),
          f >= e
            ? ((t.style.height = ""),
              (t.style.paddingTop = ""),
              (t.style.paddingBottom = ""),
              (t.style.marginTop = ""),
              (t.style.marginBottom = ""),
              (t.style.overflow = ""),
              i || (t.style.display = "none"),
              "function" == typeof o && o())
            : window.requestAnimationFrame(l);
      });
    }

    let sidebarItems = document.querySelectorAll(".sidebar-item.has-sub");
    for (var i = 0; i < sidebarItems.length; i++) {
      let sidebarItem = sidebarItems[i];
      sidebarItems[i]
        .querySelector(".sidebar-link")
        .addEventListener("click", function (e) {
          e.preventDefault();

          let submenu = sidebarItem.querySelector(".submenu");
          if (submenu.classList.contains("active"))
            submenu.style.display = "block";

          if (submenu.style.display == "none") submenu.classList.add("active");
          else submenu.classList.remove("active");
          slideToggle(submenu, 300);
        });
    }

    window.addEventListener("DOMContentLoaded", (event) => {
      var w = window.innerWidth;
      if (w < 1200) {
        document.getElementById("sidebar").classList.remove("active");
      }
    });
    window.addEventListener("resize", (event) => {
      var w = window.innerWidth;
      if (w < 1200) {
        document.getElementById("sidebar").classList.remove("active");
      } else {
        document.getElementById("sidebar").classList.add("active");
      }
    });

    document.querySelector(".burger-btn").addEventListener("click", () => {
      document.getElementById("sidebar").classList.toggle("active");
    });
    document.querySelector(".sidebar-hide").addEventListener("click", () => {
      document.getElementById("sidebar").classList.toggle("active");
    });
  },
  methods: {
    subIsActive(item) {
      const paths = Array.isArray(item.submenu) ? item.submenu : [];
      return paths.some((path) => {
        return this.$route.path.indexOf(path.url) === 0;
      });
    },

    isActive(url) {
      if (this.$route.path == url) {
        return true;
      }
      return false;
    },

    isHasSub(item) {
      if (item.hasOwnProperty("submenu")) {
        if (item.submenu.length > 0) {
          return true;
        }
      }

      return false;
    },
  },

  data() {
    return {
      items: dataSidebar,
    };
  },
};
</script>

<style lang="scss" scoped>
[class^="bi-"]::before,
[class*=" bi-"]::before {
  vertical-align: text-top;
}

ul {
  padding-left: 2rem;
}
</style>
