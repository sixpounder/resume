<template>
  <section id="contacts">
    <SectionTitle>Contact</SectionTitle>
    <div class="space-y-4 mt-4">
      <div>
        <SectionSubtitle> Phone </SectionSubtitle>
        <p>392 108 4185</p>
      </div>
      <div>
        <SectionSubtitle> Email </SectionSubtitle>
        <Email address="a.coronese@pm.me" />
      </div>
      <div>
        <SectionSubtitle> Github </SectionSubtitle>
        <a href="https://github.com/sixpounder" target="noopener">https://github.com/sixpounder</a>
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
