<template>
  <div class="skill-wrap">
    <slot />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Skill',
  props: {
    rating: {
      type: Number,
      required: false,
      default: 0,
      validator: function (value: number) {
        return value >= 0 && value <= 5;
      }
    },
    ratingLabel: {
      type: String,
      required: false,
      default: ""
    }
  }
})
</script>
