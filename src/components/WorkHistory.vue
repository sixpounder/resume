<template>
  <SectionTitle>Work history</SectionTitle>
  <section>
    <HistoryEntry
      title="Software architect / developer"
      subtitle="Monte dei Paschi di Siena, Siena, Italy"
      period="2006-10 - Current"
    >
      <ul>
        <li>
          Developed software from ground up with measured, customer-focused approach to eliminate waste and
          streamline implementation cycle
        </li>
        <li>
          Worked with a wide range of technologies, gaining proficiency in most of them, including back end analysis and development
        </li>
        <li>
          Lead designer and developer of the latest company's UI kit graphic libraries, used on the vast majority of web applications at the present day
        </li>
      </ul>
    </HistoryEntry>
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import SectionTitle from "./widgets/SectionTitle.vue";

export default defineComponent({
  components: {
    SectionTitle,
  },
});
</script>
