<template>
  <div>{{ text }}</div>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const text = ref("hola Vue");
    text.value = "nuevo contenido";
    return {
      text,
    };
  },
};
</script>
