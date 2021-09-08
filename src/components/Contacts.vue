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
        <Email address="andrea.coronese@hey.com" />
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
