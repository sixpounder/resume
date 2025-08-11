<template>
  <SectionTitle>Work history</SectionTitle>
  <section class="space-y-4">
    <HistoryEntry title="Software Architect / Developer / Tech lead" subtitle="Alten" time-range="2022-09 - Curent">
      <ul>
        <li>
          Leading a team of developers working on backend technology for a prominent client.
        </li>
        <li>
          Event driven system design & implementation.
        </li>
      </ul>
    </HistoryEntry>
    <HistoryEntry title="Software Architect / Developer" subtitle="Monte dei Paschi di Siena, Siena, Italy"
      time-range="2006-10 - 2022-09">
      <ul>
        <li>
          Developed software from ground up with measured, customer-focused
          approach to eliminate waste and streamline implementation cycle.
        </li>
        <li>
          Worked with a wide range of technologies, gaining proficiency in most
          of them, including back end analysis and development.
        </li>
        <li>
          Lead designer and developer of the latest company's UI kit graphic
          libraries, used on the vast majority of its web applications at the
          present day.
        </li>
      </ul>
    </HistoryEntry>
    <HistoryEntry title="UI/UX Designer" subtitle="Monte dei Paschi di Siena, Siena, Italy"
      time-range="2006-10 - 2022-09">
      <ul>
        <li>
          Created, improved and expanded project platforms using Javascript and
          modern web frameworks (Angular, Vue, React) to develop rich users
          interfaces.
        </li>
        <li>
          Communicated with product managers and UX designers to translate
          project requirements and business objectives into polished user
          interfaces.
        </li>
      </ul>
    </HistoryEntry>
    <HistoryEntry title="Open Source community contributor" subtitle="OSS community"
      time-range="Some point in the past - Current">
      <ul>
        <li>
          Involved in numerous open source projects of different kinds,
          including libraries like <a href="https://github.com/sixpounder/jql" target="noopener">JQL</a>, system
          utilities like <a href="https://crates.io/crates/seagul" target="noopener">Seagul</a> and free and open
          writing applications like <a href="https://github.com/sixpounder/manuscript" target="noopener">Manuscript</a>
          (soon to be published).
          For a more comprehensive list look at <a href="https://andrea-coronese.netlify.app/"
            target="noopener">andrea-coronese.netlify.app</a>.
        </li>
        <li>
          (Was) Involved into the ElementaryOS community.
        </li>
      </ul>
    </HistoryEntry>
    <HistoryEntry title="Personal Projects" subtitle="Anywhere" time-range="Continuous">
      <ul>
        <li>
          Constantly maintaining personal projects and starting new ones, both on programming and design side.
        </li>
        <li>
          Designing custom icon sets for specific purposes, either personal or for third parties.
        </li>
      </ul>
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
