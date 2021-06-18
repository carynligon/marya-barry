<template>
  <div>
    <div>
      <Nav />
      <div class="feature-img"></div>
      <div class="photo-grid container">
        <div class="img column"></div>
        <div class="img column"></div>
        <div class="img column"></div>
        <div class="img column"></div>
        <div class="img column"></div>
        <div class="img column"></div>
        <div class="img column"></div>
        <div class="img column"></div>
      </div>
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
.photo-grid {
  width: 100%;
}
.feature-img {
  border: 1px solid black;
  height: 400px;
  margin-top: var(--spacer-3xl);
}
.img {
  border: 1px solid black;
  height: 300px;
  --width: 3;
}
@media (max-width: 1200px) {
  .img {
    --width: 6;
  }
}
@media (max-width: 768px) {
  .img {
    --width: 12;
  }
}
</style>
