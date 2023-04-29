<template>
<section>
    <h1>My Skills</h1>
  <div class="logos">
    <div id="vue">
        <vueLogo></vueLogo>
        <vite></vite>
        <vutify></vutify>
        <img src="https://cdn.cosmicjs.com/85825af0-b806-11ec-a20f-432bdea59662-vuex.png" alt="vuex"  id="vuex">
    </div>
      <htmlLogo></htmlLogo>
      <css></css>
      <js></js>
    <git></git>
    <github></github>
    <sass></sass>
    <BS></BS>
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
    vutify
  },
};
</script>

<style scoped>
#vuex{
  position: relative;
  top: -1.5rem;
    width: 6rem;
}

section{
/* background-color: gray; 
background: linear-gradient(55deg ,#e8e8ec, rgb(35, 66, 177),rgb(25, 45, 116), rgb(18, 32, 85), black);*/
padding: 3rem;
text-align: center;
position: relative;
top: 20rem;
width: 100%;
}

h1{
    font-size: 3rem;
    background-color: inherit;
    color: rgb(216, 214, 214);
}

.logos{
    background-color: inherit;
}

#vue{
    background-color: inherit;
}

@media screen and (max-width: 768px) {
    section{
        width: 170%;
    }
}
</style>