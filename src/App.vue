<script lang="ts">
import { defineComponent } from "vue";
import Header from "./components/resume/Header.vue";
import Layout from "./components/resume/Layout.vue";
import Footer from "./components/resume/Footer.vue";
import Prologue from "./components/resume/Prologue.vue";
import WorkHistory from "./components/resume/WorkHistory.vue";
import Education from "./components/resume/Education.vue";
import Contacts from "./components/resume/Contacts.vue";
import Skills from "./components/resume/Skills.vue";
import SpokenLanguages from "./components/resume/Languages.vue";
import SoftSkills from "./components/resume/SoftSkills.vue";

export default defineComponent({
  components: {
    Header,
    Layout,
    Footer,
    Prologue,
    WorkHistory,
    Education,
    Contacts,
    Skills,
    SpokenLanguages,
    SoftSkills,
  },
});
</script>

<template>
  <main class="md:container md:mx-auto">
    <Header />
    <Layout>
      <template v-slot:left>
        <Prologue />
        <WorkHistory />
        <Education />
      </template>
      <template v-slot:right>
        <Contacts />
        <Skills />
        <SoftSkills />
        <SpokenLanguages />
        <Footer />
      </template>
    </Layout>
  </main>
</template>
