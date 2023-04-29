<template>
  <section>
    <p v-motion-slide-visible-left>Uriel Kasabe</p>
    <img src="../../media/uri.jpg" alt="profile picture"  v-motion-roll-visible-right/>
    <div>
      <h1>About me</h1>
      <h2>
        A Self learner and dedicated Frontend developer with a high self
        discipline, willing to increase my limits and my knowledge.
      </h2>
    </div>
    <div>
      <h1>Why me?</h1>
      <h2>
        very kind and proffessional, looking always to get the job done in the
        minor time, want to learn new tecnologies and give others from my
        knowledge. dedicated and always think about how the product could be the
        bestest.
      </h2>
    </div>
  </section>
</template>

<style scoped>
section {
  background: inherit;
  padding: 3rem;
  text-align: center;
  position: relative;
  top: 20rem;
  width: 100%;
  color: rgb(216, 214, 214);
}

div {
  margin: 5rem auto 5rem auto;
  width: 80%;
}

p {
  font-size: 2rem;
  margin: 1rem;
  color: rgb(216, 214, 214);
  text-align: center;
}

h1 {
  color: rgb(89, 227, 89);
  font-size: 1.5rem;
}

img {
  position: relative;
  top: 0.2rem;
  left: 0;
  height: 14rem;
  width: 14rem;
  border: none;
  border-radius: 50%;
  margin: 0 auto;
  display: block;
  align-content: center;
}

@media screen and (max-width: 768px) {
    section{
        width: 40rem;
        left: 35%;
        transform: translateX(-18%);
    }

    div{
        width: 100%;
    }
}
</style>
