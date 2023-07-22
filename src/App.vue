<template>
  <galaxy></galaxy>
  <div class="container">
    <h1 class="line-1 anim-typewriter">Uriel Kasabe</h1>
    <hr />
    <h2 class="desc anim">
      Frontend developer specilized in <span class="vue">Vue.js</span>
    </h2>
  </div>
  <upButton></upButton>
  <about> </about>
  <Theskills></Theskills>

  <footer>
    <foot> </foot>
  </footer>
</template>

<script>
import galaxy from './components/backgroundGalaxy.vue';
import Theskills from './components/mySkills.vue';
import about from './components/AboutMe.vue';
import foot from './components/layouts/TheFooter.vue';
import upButton from './components/UpButton.vue';

export default{
  components: {
    Theskills,
    galaxy,
    about,
    foot,
    upButton,

  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Bruno+Ace+SC&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Bruno Ace SC', cursive;
}

body {
  margin: 0;
}

.container {
  font-family: 'Bruno Ace SC', cursive;
  margin-top: 20rem;
  text-align: center;
  align-content: center;
}

.vue {
  color: rgb(89, 227, 89);
}

hr {
  margin-top: 0.1rem;
  margin-bottom: 3rem;
  border: 1px solid white;
  width: 30%;
}

.line-1 {
  position: relative;
  top: 50%;
  left: 0;
  width: 100%;
  margin: 0 auto;
  border-right: 2px solid rgba(255, 255, 255, 0.75);
  color: rgb(216, 214, 214);
  font-size: 4rem;
  text-align: center;
  white-space: nowrap;
  overflow: hidden;
  transform: translateY(-50%);
}

.desc {
  color: rgb(188, 187, 187);
  position: relative;
  top: 50%;
  left: 0;
  width: 100%;
  margin: 0 auto;
  border-right: 2px solid rgba(255, 255, 255, 0.75);
  text-align: center;
  white-space: nowrap;
  overflow: hidden;
  transform: translateY(-50%);
}

/* Animation */
.anim-typewriter {
  animation: typewriter 2s steps(20) 1s 1 normal both,
    blinkTextCursor 500ms steps(20) infinite normal;
}

.anim {
  animation: typedesc 3s steps(25) 3s 1 normal both,
    blinkTextCursor 500ms steps(25) infinite normal;
}

@keyframes typewriter {
  from {
    width: 0;
  }
  to {
    width: 8em;
  }
}
@keyframes blinkTextCursor {
  from {
    border-right-color: rgba(255, 255, 255, 0.75);
  }
  to {
    border-right-color: transparent;
  }
}
@keyframes typedesc {
  from {
    width: 0;
  }
  to {
    width: 25em;
  }
}

@media screen and (max-width: 768px) {
  .container {
    margin: 9rem 1rem 0 1rem;
    width: fit-content;
  }

  .line-1 {
    top: 7rem;
    left: 14%;
  }

  .desc {
    top: 7rem;
    left: 14%;
    display: flex;
    flex-direction: column;
  }

  hr {
    position: relative;
    top: 7rem;
    left: 15%;
    width: 70%;
    margin-bottom: 5rem;
  }

  footer {
    width: 43.8rem;
  }

  @keyframes typedesc {
    from {
      width: 0;
    }
    to {
      width: 20.5em;
    }
  }
}
</style>
