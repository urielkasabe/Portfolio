<template>
  <section>
    <h1>My Skills</h1>
    <div class="logos">
      <div id="vue">
        <vueLogo v-motion-pop-visible-once></vueLogo>
        <vite v-motion-pop-visible-once></vite>
        <vutify v-motion-pop-visible-once></vutify>
        <img
          src="https://cdn.cosmicjs.com/85825af0-b806-11ec-a20f-432bdea59662-vuex.png"
          alt="vuex"
          id="vuex"
          v-motion-pop-visible-once
        />
      </div>
      <htmlLogo v-motion-pop-visible-once></htmlLogo>
      <css v-motion-pop-visible-once></css>
      <js v-motion-pop-visible-once></js>
      <git v-motion-pop-visible-once></git>
      <github v-motion-pop-visible-once></github>
      <sass v-motion-pop-visible-once></sass>
      <BS v-motion-pop-visible-once></BS>
      <div>
        <img
          v-motion-pop-visible-once
          width="152"
          alt="Node.js logo"
          src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Node.js_logo.svg/128px-Node.js_logo.svg.png"
        />
      </div>
    </div>
  </section>
</template>

<script>
import vueLogo from '../svgs/vueLogo.vue';
import htmlLogo from '../svgs/htmlLogo.vue';
import css from '../svgs/css-3.vue';
import js from '../svgs/logo-javascript.vue';
import git from '../svgs/git.vue';
import github from '../svgs/github-icon-1.vue';
import sass from '../svgs/sass-1.vue';
import BS from '../svgs/bootstrap-5-1.vue';
import vite from '../svgs/vitejs.vue';
import vutify from '../svgs/vuetify.vue';

export default {
  components: {
    vueLogo,
    htmlLogo,
    css,
    js,
    git,
    github,
    sass,
    BS,
    vite,
    vutify,
  },
};
</script>

<style scoped>
#vuex {
  position: relative;
  top: -1.5rem;
  width: 6rem;
  filter: drop-shadow(1.5rem 0 0.3rem rgb(0, 0, 0));
}

section {
  padding: 3rem;
  text-align: center;
  position: relative;
  top: 20rem;
  width: 100%;
}

h1 {
  font-size: 3rem;
  background-color: inherit;
  color: rgb(216, 214, 214);
}

.logos {
  background-color: inherit;
}

#vue {
  background-color: inherit;
}

@media screen and (max-width: 768px) {
  section {
    width: 170%;
  }
}
</style>
