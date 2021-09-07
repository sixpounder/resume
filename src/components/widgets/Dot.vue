<template>
  <svg :viewBox="viewBox" :style="style">
    <circle
      :cx="computedSize / 2"
      :cy="computedSize / 2"
      :r="computedSize / 2"
      :fill="computedColor"
      :stroke="computedColor"
      stroke-width="0"
    />
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
    },

    color: {
      type: String,
      required: false,
      default: '#000000'
    }
  },

  computed: {
    computedSize (): number {
      return this.size ?? 20
    },

    computedColor (): string {
      return this.active ? this.color : `${this.color}40`;
    },

    viewBox () {
      return `0 0 ${this.computedSize} ${this.computedSize}`
    },

    style () {
      return {
        height: `${this.computedSize}px`
      }
    }
  }
})
</script>
