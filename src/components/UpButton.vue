<template>
  <button @click="upScroll" v-if="scrolled > 0" class="btn-up">
    <el-icon style="font-size: 2.5rem"><Top /></el-icon>
  </button>
</template>

<script>
export default {
  data() {
    return {
      scrolled: null,
    };
  },
  methods: {
    handleScroll() {
      this.scrolled = window.scrollY > 0;
    },
    upScroll() {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    },
  },
  created() {
    window.addEventListener('scroll', this.handleScroll);
  },
  unmounted() {
    window.removeEventListener('scroll', this.handleScroll);
  },
};
</script>

<style scoped>
.btn-up {
  cursor: pointer;
  position: fixed;
  left: 92%;
  top: 85%;
  align-items: center;
  color: rgb(50, 49, 49);
  z-index: 5;
  height: 4rem;
  width: 4rem;
  border-radius: 50%;
  background-color: rgba(254, 254, 255, 0.4);
  border: 0;
}

.btn-up:hover {
  background-color: rgba(255, 255, 255, 0.671);
}

.el-icon {
  margin: 0 auto;
  background-color: transparent;
  transform: translateY(10%);
  color: rgb(12, 12, 12);
}

.el-icon svg {
  margin: 0;
  filter: none;
}

@media screen and (max-width: 768px) {
  .btn-up {
    left: 88%;
    top: 85%;
  }
}
</style>
