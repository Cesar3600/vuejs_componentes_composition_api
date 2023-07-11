<template>
  <button @click="show = !show">MENU</button>
  <transition name="fade">
    <MainMenu v-show="show" />
  </transition>
</template>

<script>
import MainMenu from "./components/MainMenu.vue";
export default {
  name: "App",
  components: { MainMenu },
  data() {
    return {
      show: false,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.3s ease;
}
</style>
