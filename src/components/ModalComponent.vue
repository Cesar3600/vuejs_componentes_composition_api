<template>
  <div class="content-modal">
    <button @click="toggle">Modal</button>
    <teleport to="body">
      <div v-show="show" class="modal">
        <h1>titulo</h1>
        <p>lorem ipsum</p>
        <button @click="toggle">cerrar</button>
      </div>
    </teleport>
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
