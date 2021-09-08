<script lang="ts">
import { defineComponent } from "vue";
import Header from "./components/Header.vue";
import Layout from "./components/Layout.vue";
import Footer from "./components/Footer.vue";
import Prologue from "./components/Prologue.vue";
import WorkHistory from "./components/WorkHistory.vue";
import Education from "./components/Education.vue";
import Contacts from "./components/Contacts.vue";
import Skills from "./components/Skills.vue";
import SpokenLanguages from "./components/Languages.vue";

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
        <SpokenLanguages />
        <Footer />
      </template>
    </Layout>
  </main>
</template>

<style lang="stylus">
a
  @apply text-indigo-600
  &:hover
      @apply underline

  @media print
    color initial
    &:hover
        text-decoration none
</style>
