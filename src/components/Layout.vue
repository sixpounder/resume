<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Layout",
});
</script>

<template>
  <div class="flex flex-row">
    <div class="flex-1 flex-grow p-6">
      <slot name="left" />
    </div>
    <div class="flex-0 bg-gray-300 p-6">
      <slot name="right" />
    </div>
  </div>
</template>
