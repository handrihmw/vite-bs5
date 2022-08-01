<template>
  <div class="d-flex gap-5">
    <div class="pre-card">
      <div class="pre-card-header">
        <h4 class="as-text-20-semibold">Top Tooltip</h4>
      </div>
      <div class="pre-card-body">
        <p class="as-color-secondary">
          Use the
          <code>.as-tooltip, .as-tooltip__info, .as-tooltip__info--top</code>
          classes
        </p>
        <div class="as-mt-16">
          <AsTooltip>
            <AsTooltipInfo top text="label 1"></AsTooltipInfo>
          </AsTooltip>
        </div>
      </div>
    </div>

    <div class="pre-card">
      <div class="pre-card-header">
        <h4 class="as-text-20-semibold">Bottom Tooltip</h4>
      </div>
      <div class="pre-card-body">
        <p class="as-color-secondary">
          Use the
          <code>.as-tooltip, .as-tooltip__info, .as-tooltip__info--bottom</code>
          classes
        </p>
        <div class="as-mt-16">
          <AsTooltip>
            <AsTooltipInfo bottom text="label 2"></AsTooltipInfo>
          </AsTooltip>
        </div>
      </div>
    </div>
  </div>

  <div class="d-flex gap-5">
    <div class="pre-card">
      <div class="pre-card-header">
        <h4 class="as-text-20-semibold">Right Tooltip</h4>
      </div>
      <div class="pre-card-body">
        <p class="as-color-secondary">
          Use the
          <code>.as-tooltip, .as-tooltip__info, .as-tooltip__info--right</code>
          classes
        </p>
        <div class="as-mt-16">
          <AsTooltip>
            <AsTooltipInfo right text="label 2"></AsTooltipInfo>
          </AsTooltip>
        </div>
      </div>
    </div>

    <div class="pre-card">
      <div class="pre-card-header">
        <h4 class="as-text-20-semibold">Left Tooltip</h4>
      </div>
      <div class="pre-card-body">
        <p class="as-color-secondary">
          Use the
          <code>.as-tooltip, .as-tooltip__info, .as-tooltip__info--left</code>
          classes
        </p>
        <div class="as-mt-16">
          <AsTooltip>
            <AsTooltipInfo left text="label 2"></AsTooltipInfo>
          </AsTooltip>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import AsTooltip from "./AsTooltip.vue";
import AsTooltipInfo from "./AsTooltipInfo.vue";
</script>
