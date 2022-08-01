<template>
  <div class="col-md-8">
    <AsCard>
      <AsCardHeader>
        <h2 class="as-text-24-bold">Information Resource</h2>
      </AsCardHeader>
      <AsCardContainer>
        <div class="row as-mb-24">
          <div class="col-md-6 as-pr-24">
            <p class="as-text-14 as-color-disable as-mb-8">Inodes Usage</p>
            <p class="as-text-20 as-color-secondary as-mb-8">
              <span class="as-text-bold as-color-primary">1</span> dari 750,000
            </p>
            <AsProgress>
              <AsProgressBar
                valuenow="50"
                valuemin="0"
                valuemax="100"
              ></AsProgressBar>
            </AsProgress>
          </div>
          <div class="col-md-6 as-pr-24">
            <p class="as-text-14 as-color-disable as-mb-8">
              Physical Memory Usage
            </p>
            <p class="as-text-20 as-color-secondary as-mb-8">
              <span class="as-text-bold as-color-primary">0,93 MB</span> dari
              768 MB
            </p>
            <AsProgress>
              <AsProgressBar
                valuenow="20"
                valuemin="0"
                valuemax="100"
              ></AsProgressBar>
            </AsProgress>
          </div>
        </div>
        <div class="row as-mb-24">
          <div class="col-md-6">
            <p class="as-text-14 as-color-disable">Disk Space</p>
            <div class="d-flex align-items-center justify-content-between">
              <p
                class="as-text-20 as-color-secondary d-flex align-items-center gap-2"
              >
                <span class="as-text-bold as-color-primary">1 MB</span> dari
                <i class="as-icon-unlimited as-icon-gray"></i>
              </p>
              <a href="#" class="as-link as-text-14 as-btn-icon"
                ><span>Lihat Detail</span><i class="as-icon-arrow-right"></i
              ></a>
            </div>
          </div>
          <div class="col-md-6">
            <p class="as-text-14 as-color-disable">Email Accounts</p>
            <div class="d-flex align-items-center justify-content-between">
              <p
                class="as-text-20 as-color-secondary d-flex align-items-center gap-2"
              >
                <span class="as-text-bold as-color-primary">1</span> dari
                <i class="as-icon-unlimited as-icon-gray"></i>
              </p>
              <a href="#" class="as-link as-text-14 as-btn-icon"
                ><span>Lihat Detail</span><i class="as-icon-arrow-right"></i
              ></a>
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col-md-6">
            <p class="as-text-14 as-color-disable">Bandwith</p>
            <div class="d-flex align-items-center justify-content-between">
              <p
                class="as-text-20 as-color-secondary d-flex align-items-center gap-2"
              >
                <span class="as-text-bold as-color-primary">1 MB</span> dari
                <i class="as-icon-unlimited as-icon-gray"></i>
              </p>
              <a href="#" class="as-link as-text-14 as-btn-icon"
                ><span>Lihat Detail</span><i class="as-icon-arrow-right"></i
              ></a>
            </div>
          </div>
          <div class="col-md-6">
            <p class="as-text-14 as-color-disable">MySQL Database</p>
            <div class="d-flex align-items-center justify-content-between">
              <p
                class="as-text-20 as-color-secondary d-flex align-items-center gap-2"
              >
                <span class="as-text-bold as-color-primary">1</span> dari
                <i class="as-icon-unlimited as-icon-gray"></i>
              </p>
              <a href="#" class="as-link as-text-14 as-btn-icon"
                ><span>Lihat Detail</span><i class="as-icon-arrow-right"></i
              ></a>
            </div>
          </div>
        </div>
      </AsCardContainer>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardHeader from "./AsCardHeader.vue";

import AsProgress from "../progress/AsProgress.vue";
import AsProgressBar from "../progress/AsProgressBar.vue";
</script>
