<template>
  <section id="contacts">
    <SectionTitle>Contact</SectionTitle>
    <div class="space-y-4 mt-4">
      <div>
        <SectionSubtitle> Email </SectionSubtitle>
        <Email address="a.coronese@pm.me" />
      </div>
      <div>
        <SectionSubtitle> Github </SectionSubtitle>
        <a href="https://github.com/sixpounder" target="noopener">github.com/sixpounder</a>
      </div>
      <div>
        <SectionSubtitle> Website </SectionSubtitle>
        <a href="https://andrea-coronese.netlify.app/" target="noopener">andrea-coronese.netlify.app</a>
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import SectionTitle from "./widgets/SectionTitle.vue";
import SectionSubtitle from "./widgets/SectionSubtitle.vue";
import Email from "./widgets/Email.vue";

export default defineComponent({
  components: {
    SectionTitle,
    SectionSubtitle,
    Email,
  },
});
</script>
