<template>
  <div>
    <button @click="toggle">Modal</button>
    <div v-show="show" class="modal">
      <h1>titulo</h1>
      <p>lorem ipsum</p>
      <button @click="toggle">cerrar</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      show: false,
    };
  },
  methods: {
    toggle() {
      this.show = !this.show;
    },
  },
};
</script>
