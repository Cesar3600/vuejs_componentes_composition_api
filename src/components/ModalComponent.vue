<template>
  <div>{{ text }}</div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      text: "Hola VUE",
    };
  },
  beforeCreate() {
    console.log("beforeCreate", this.$data, this.$el);
  },
  created() {
    console.log("created", this.$data, this.$el);
  },
  mounted() {
    console.log("mounted", this.$data, this.$el);
  },
};
</script>

<style>
.content-modal {
  width: 100vw;
  height: 100vh;
}
.modal {
  width: 100%;
  max-width: 300px;
  display: flex;
  flex-direction: column;
  gap: 2rem;
}
h1 {
  text-transform: uppercase;
}
</style>
