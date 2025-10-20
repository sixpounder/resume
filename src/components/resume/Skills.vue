<template>
  <section id="skills">
    <SectionTitle>Skills</SectionTitle>
    <div class="mt-4 space-y-4">
      <Skill :rating="5">Javascript / Typescript</Skill>
      <Skill :rating="5">API Design</Skill>
      <Skill :rating="5">UI/UX Design</Skill>
      <Skill :rating="5">Angular</Skill>
      <Skill :rating="5">React</Skill>
      <Skill :rating="5">Vue</Skill>
      <Skill :rating="5">NodeJS</Skill>
      <Skill :rating="5">Web design</Skill>
      <Skill :rating="5">Java</Skill>
      <Skill :rating="5">Spring Boot</Skill>
      <Skill :rating="5">Kafka Streams / Connect</Skill>
      <Skill :rating="5">Rust</Skill>
      <Skill :rating="4">Ruby</Skill>
      <Skill :rating="4">Mongo</Skill>
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
