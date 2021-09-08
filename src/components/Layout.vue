<template>
  <div class="layout-wrap flex flex-col md:flex-row">
    <div class="left-wrapper">
      <slot name="left" />
    </div>
    <div class="right-wrapper break-words">
      <slot name="right" />
    </div>
  </div>
</template>

<style lang="stylus" scoped>
  .layout-wrap
    .left-wrapper
      @apply flex-auto p-6 text-justify break-words space-y-8

    .right-wrapper
      @apply flex-1 flex-shrink bg-gray-200 p-6 space-y-8
      min-width 25%
</style>
