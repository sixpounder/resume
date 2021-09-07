<script lang="ts">
import { defineComponent } from "vue";
import Header from "./components/Header.vue";
import Layout from "./components/Layout.vue";
import Footer from "./components/Footer.vue";

export default defineComponent({
  components: {
    Header,
    Layout,
    Footer
  },
});
</script>


<template>
  <Header />
  <Layout>
    <template v-slot:left>Left</template>
    <template v-slot:right>Left</template>
  </Layout>
  <Footer />
</template>
