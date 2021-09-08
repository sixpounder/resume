<template>
  <section id="spoken-languages">
    <SectionTitle>Spoken languages</SectionTitle>
    <div class="mt-4 space-y-4">
      <Skill :rating="5" rating-label="Mother tongue">Italian</Skill>
      <Skill :rating="5">English</Skill>
    </div>
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import SectionTitle from "./widgets/SectionTitle.vue";
import Skill from './widgets/Skill.vue';

export default defineComponent({
  components: {
    SectionTitle,
    Skill,
  },
});
</script>
