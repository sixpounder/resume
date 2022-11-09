<template>
  <SectionTitle>Education</SectionTitle>
  <section class="space-y-4">
    <HistoryEntry
      title="High School Diploma"
      subtitle="ITIS Tito Sarrocchi - Siena, Italy"
      time-range="1998 - 2003"
    >
    </HistoryEntry>
    <HistoryEntry
      title="J.D. Computer Science and Programming"
      subtitle="Università degli Studi di Siena - Siena, Italy"
      time-range="2003-10 - Current"
    >
    </HistoryEntry>
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import SectionTitle from "./widgets/SectionTitle.vue";
import HistoryEntry from "./widgets/HistoryEntry.vue";

export default defineComponent({
  components: {
    SectionTitle,
    HistoryEntry,
  },
});
</script>

<style lang="stylus" scoped>
ul {
  @apply: list-disc;
}
</style>
