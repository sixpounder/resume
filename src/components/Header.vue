<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Header",
});
</script>

<template>
  <header>
    <h1>Andrea Coronese</h1>
    <h2>Software Architect & Developer - UI/UX Designer</h2>
  </header>
</template>

<style lang="stylus" scoped>
header {
  @apply: bg-gray-800 p-6;

  h1 {
    @apply: text-6xl my-3 text-gray-200 font-bold tracking-wide;
  }

  h2 {
    @apply: text-3xl my-3 text-gray-400 font-light tracking-wide;
  }
}
</style>
