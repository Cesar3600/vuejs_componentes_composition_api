<template>
  <div>{{ text }}</div>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const text = ref("hola Vue");
    return {
      text,
    };
  },
};
</script>
