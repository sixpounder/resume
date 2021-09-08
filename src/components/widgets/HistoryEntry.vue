<template>
  <div class="history-entry-layout">
    <div class="time-wrap">
      <p v-if="timeRange">
        {{ timeRange }}
      </p>
    </div>
    <div class="content-wrap">
      <section-subtitle v-if="title">{{ title }}</section-subtitle>
      <i v-if="subtitle">{{ subtitle }}</i>
      <slot />
    </div>
  </div>
</template>

<script lang="ts" setup>
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
  timeRange: {
    type: String,
    required: false,
    default: undefined
  }
})
</script>

<script lang="ts">
import { defineComponent } from 'vue'
import SectionSubtitle from './SectionSubtitle.vue'

export default defineComponent({
  components: { SectionSubtitle },
  name: "HistoryEntry"
})
</script>

<style lang="stylus" scoped>
.history-entry-layout
  @apply flex flex-row space-x-8
  .content-wrap
    @apply flex-1
  .time-wrap
    width 20%
    @apply font-bold
</style>
