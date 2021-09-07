<template>
  <svg :width="computedSize" :height="computedSize">
    <circle cx="50" cy="50" r="40" :stroke="computedColor" stroke-width="4" fill="yellow" />
  </svg>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    active: {
      type: Boolean,
      required: false,
      default: false
    },

    size: {
      type: Number,
      required: false,
      default: 20
    }
  },

  computed: {
    computedSize (): number {
      return this.size ?? 20
    },

    computedColor (): string {
      return this.active ? '' : ''
    }
  }
})
</script>
