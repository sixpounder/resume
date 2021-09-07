<template>
  <h4>
    <slot />
  </h4>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "SectionSubtitle",
});
</script>

<style lang="stylus" scoped>
  h4
    @apply text-xl font-bold
</style>
