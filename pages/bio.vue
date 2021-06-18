<template>
  <div>
    <div>
      <Nav />
      <ContentSection
        v-for="section in copy.sections"
        v-bind:copy="section"
        v-bind:key="section.title"
      />
    </div>
    <Footer />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import copy from "~/copy/bio";
import Nav from "~/components/Nav.vue";
import ContentSection from "~/components/ContentSection.vue";
import Footer from "~/components/Footer.vue";

export default Vue.extend({
  components: {
    Nav,
    ContentSection,
    Footer,
  },
  data() {
    return {
      copy,
    };
  },
});
</script>

<style>
.content {
  margin-top: var(--spacer-2xl);
}
.content-sub.no-title {
  margin-top: 0;
}
</style>
