<template>
  <section>
    <p v-motion-slide-visible-once-left class="title">About Me</p>
    <img src="../../media/uri.jpg" alt="profile picture"  v-motion-roll-visible-once-right/>
    <div class="container-about">
    <div v-motion-pop-visible-once>
      <h1>Who am I?</h1>
      <h2>
        A Self learner and dedicated Frontend developer with a high self
        discipline, willing to increase my limits and my knowledge.
      </h2>
      <h2>
        very kind and proffessional, looking always to get the job done in the
        minority of time, want to learn new tecnologies and give others from my
        knowledge. self - discipline and always think about how can I take the product to the highest level.
      </h2>
    </div>
    <div v-motion-pop-visible-once>
      <h1>Uriel Kasabe</h1>
      <p><span>E-Mail:</span>  urielkasabe5@gmail.com</p>
      <p><span>Phone:</span>  +972528776372</p>
      <p><span>City:</span>  Ra'anana, Israel</p>
      <p><span>Languages:</span> English, Spanish, Hebrew, Italian</p>
    </div>
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
  margin: 5rem;
  width: 90%;
}

.container-about{
display: flex;
text-align: left;
margin-bottom: 0;
margin-top: 0;
}

.title {
  font-size: 3rem;
  background-color: inherit;
  color: rgb(216, 214, 214);
}

h1 {
  color: rgb(89, 227, 89);
  font-size: 1.5rem;
}

h2{
  font-size: 1rem;
}

p{
  margin: 1.8rem auto;
}

span{
  font-size: 1.1rem;
  color: rgb(42, 155, 42);
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
        transform: translateX(-18%);
    }
    .title{
     position: relative;
      left: 27.5%; 
    }

    img{
      left: 27.5%;
    }

    div{
        width: 100%;
        margin-bottom: 0;
    }

    .container-about{
      flex-direction: column;
      text-align: center;
    }
}
</style>
