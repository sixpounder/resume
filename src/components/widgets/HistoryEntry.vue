<template>
  <div class="flex flex-row">
    <div></div>
    <div>
      <slot />
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps({
  title: {
    type: String,
    required: false,
    default: undefined
  },
  subtitle: {
    type: String,
    required: false,
    default: undefined
  },
  period: {
    type: String,
    required: false,
    default: undefined
  }
})
</script>
