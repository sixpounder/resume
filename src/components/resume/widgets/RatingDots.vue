<template>
  <div class="inline-flex flex-row flex-grow-0 space-x-1 justify-end">
    <Dot v-for="index in 5" :key="index" :active="index <= value" :size="16" :color="color"></Dot>
  </div>
</template>

<script lang="ts" setup>
import Dot from './Dot.vue';

defineProps({
  value: {
    type: Number,
    required: true,
    validator: function (value: number) {
      return value >= 0 && value <= 5;
    },
  },
  color: {
    type: String,
    required: false,
    default: "#f59e0b"
  }
});
</script>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: "RatingDots"
})
</script>
