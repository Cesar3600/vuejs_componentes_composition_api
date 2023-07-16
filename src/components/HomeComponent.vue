<template>
  <div>{{ encendido ? "abierto" : "cerrado" }}</div>
  <button v-on:click="toggle">encender/ apagar</button>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const encendido = ref(true);
    const toggle = () => {
      encendido.value = !encendido.value;
    };
    return {
      encendido,
      toggle,
    };
  },
};
</script>
