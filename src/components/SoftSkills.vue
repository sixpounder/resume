<template>
  <section id="soft-skills">
    <SectionTitle>Soft Skills</SectionTitle>
    <div class="mt-4 space-y-4">
      <Skill :rating="5">Problem solving</Skill>
      <Skill :rating="5">Creativity</Skill>
      <Skill :rating="5">Critical Thinking</Skill>
      <Skill :rating="4">Negotiation</Skill>
      <Skill :rating="4">Lateral Thinking</Skill>
      <Skill :rating="4">Team management</Skill>
      <Skill :rating="4">Stress management</Skill>
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
