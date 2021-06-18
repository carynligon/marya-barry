<template>
  <div>
    <div>
      <Nav />
      Reviews
    </div>
    <Footer />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import copy from "~/copy/resume";
import Nav from "~/components/Nav.vue";
import ContentSection from "~/components/ContentSection.vue";
import Footer from "~/components/Footer.vue";

export default Vue.extend({
  components: {
    Nav,
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
