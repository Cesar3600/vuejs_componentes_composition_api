<template>
  <Home
    firstName="Catherine"
    lastName="Mikaela"
    alias="mi amor verdadero"
  ></Home>
</template>
<script>
import Home from "@/components/HomeComponent.vue";
export default {
  name: "App",
  components: { Home },
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  padding: 0px;
  margin: 0;
}
#app > div {
  padding: 2rem;
}
</style>
