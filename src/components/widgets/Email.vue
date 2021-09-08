<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Email",
  props: {
    address: {
      type: String,
      required: true
    }
  },
  computed: {
    addressHref () {
      return `mailto:${this.address.toLowerCase()}`
    }
  }
});
</script>

<template>
  <a :href="addressHref">
    {{ address }}
  </a>
</template>

<style lang="stylus" scoped>
  a
    @media screen
      @apply text-indigo-600
      &:hover
        @apply underline
    @media print
      color initial
</style>
