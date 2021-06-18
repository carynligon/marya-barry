<template>
  <div class="container">
    <div>
      <Nav />
      <h1 class="title column">
        I’m Marya Barry, an opera director and makeup artist in Knoxville, TN.
      </h1>
      <div class="feature-img"></div>
      <div class="roles container">
        <div class="current-role column">
          <h3>Email</h3>
          <div class="role-content">
            <!-- <p class="current-role-text">UX Designer @ IBM, since 2018</p> -->
            <div class="email">
              <p>maryabarry92@gmail.com</p>
              <textarea
                id="email-copy"
                disabled="true"
                value="maryabarry92@gmail.com "
                style="opacity: 0; position: absolute;"
              >
maryabarry92@gmail.com </textarea
              >
              <div
                v-bind:class="{
                  ['email-svg-wrapper']: true,
                  hover: hover,
                }"
                v-on:click="copyEmail"
              >
                <img
                  alt="click to copy email address"
                  src="~/assets/svgs/copy.svg"
                />
                <div class="copy-text">{{ copyText }}</div>
              </div>
            </div>
          </div>
        </div>
        <div class="previous-roles column">
          <h3>Contact Form</h3>
          <form class="role-content">
            <input type="text" />
          </form>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import Nav from "~/components/Nav.vue";
import Footer from "~/components/Footer.vue";

export default Vue.extend({
  components: {
    Nav,
    Footer,
  },
  methods: {
    setHoverState() {
      this.copyText = "Copied!";
      this.hover = true;
      const hoverTimeout = setTimeout(() => {
        this.hover = false;
        clearTimeout(hoverTimeout);
      }, 1300);
      const textTimeout = setTimeout(() => {
        this.copyText = "Copy email";
        clearTimeout(textTimeout);
      }, 1500);
    },
    copyEmail() {
      if (navigator.clipboard && navigator.clipboard.writeText) {
        navigator.clipboard.writeText("hello@derrickligon.com");
        return this.setHoverState();
      }
      const inputEl = document.getElementById("email-copy") || {};
      // @ts-ignore
      inputEl.select();
      document.execCommand("copy");
      return this.setHoverState();
    },
  },
  data() {
    return {
      copyText: "Copy email",
      hover: false,
    };
  },
});
</script>

<style>
body {
  font-family: "Graphik Web";
}
.title {
  font-weight: normal;
  line-height: 3.625rem;
  margin: 5.625rem 0 3.0625rem 0;
  --width: 12;
}
.roles p {
  font-size: var(--font-size-body-lg);
}
h3 {
  font-size: var(--font-size-h3);
  font-weight: normal;
  margin-bottom: var(--spacer-xs);
}
.spacer {
  --width: 1;
}
.current-role,
.previous-roles {
  --width: 6;
}
.role-content {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.current-role-text {
  margin-bottom: var(--spacer-lg);
}
.previous-roles ul {
  padding: 0;
}
.email {
  align-items: center;
  display: flex;
}
.roles .email p {
  margin: 0;
}
.email .email-svg-wrapper {
  align-items: center;
  border-radius: 4px;
  display: flex;
  height: 2.25rem;
  justify-content: center;
  margin-left: 6px;
  position: relative;
  width: 2.25rem;
}
.copy-text {
  background-color: var(--black);
  border-radius: 4px;
  color: #fff;
  content: "Copy email";
  display: block;
  font-size: 0.75rem;
  opacity: 0;
  padding: 0.375rem 0.5rem;
  position: absolute;
  top: 1.75rem;
  transition: 150ms all cubic-bezier(0.4, 0, 0.2, 1);
  white-space: nowrap;
}
.email-svg-wrapper:hover .copy-text,
.email-svg-wrapper.hover .copy-text {
  opacity: 1;
  top: 2.5rem;
  transition: 150ms all cubic-bezier(0.4, 0, 0.2, 1);
}
.email img {
  height: 1.25rem;
  width: 1.25rem;
}
.email .email-svg-wrapper:hover {
  cursor: pointer;
  background-color: rgba(0, 0, 0, 0.04);
}

@media (max-width: 992px) {
  .current-role,
  .previous-roles {
    --width: 12;
  }
  .roles p {
    margin-bottom: var(--spacer-xs);
  }
  .previous-roles {
    margin-top: var(--spacer-lg);
  }
}
@media (max-width: 576px) {
  .title {
    line-height: var(--font-size-h1);
    margin-top: var(--spacer-3xl);
  }
}
</style>
