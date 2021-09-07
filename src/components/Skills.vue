<template>
  <section id="skills">
    <SectionTitle>Skills</SectionTitle>
    <div class="mt-4 space-y-4">
      <Skill :rating="5">Javascript / Typescript Specialist</Skill>
      <Skill :rating="5">API design Specialist</Skill>
      <Skill :rating="5">UI/UX Design</Skill>
      <Skill :rating="5">Modern Front End Web Development</Skill>
      <Skill :rating="5">NodeJS Expert</Skill>
      <Skill :rating="5">Web design</Skill>
      <Skill :rating="4">Rust</Skill>
      <Skill :rating="4">Ruby</Skill>
      <Skill :rating="3">C/C++</Skill>
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
