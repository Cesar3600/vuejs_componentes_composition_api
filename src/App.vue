<template>
  <UserRepositories :user="'Diana'"></UserRepositories>
</template>

<script>
import UserRepositories from "./components/UserRepositories.vue";

export default {
  name: "App",
  components: { UserRepositories },
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
