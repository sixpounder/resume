<script lang="ts">
import { defineComponent } from "vue";
import Header from "./components/Header.vue";
import Layout from "./components/Layout.vue";
import Footer from "./components/Footer.vue";
import Prologue from "./components/Prologue.vue";
import WorkHistory from "./components/WorkHistory.vue";
import Contacts from "./components/Contacts.vue";
import Skills from "./components/Skills.vue";

export default defineComponent({
  components: {
    Header,
    Layout,
    Footer,
    Prologue,
    WorkHistory,
    Contacts,
    Skills
  },
});
</script>

<template>
  <Header />
  <Layout>
    <template v-slot:left>
      <Prologue />
      <WorkHistory />
      <Footer class="mt-60" />
    </template>
    <template v-slot:right>
      <Contacts />
      <Skills />
    </template>
  </Layout>
</template>
