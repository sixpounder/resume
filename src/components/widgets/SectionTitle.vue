<template>
  <h3>
    <slot />
  </h3>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "SectionTitle",
});
</script>

<style lang="stylus" scoped>
  h3
    @apply text-3xl pb-2 font-bold border-b border-gray-400
</style>
