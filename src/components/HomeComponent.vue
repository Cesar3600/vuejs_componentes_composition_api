<template>
  <div>{{ obj }}</div>
</template>

<script>
import { watch, ref } from "vue";
export default {
  setup() {
    const obj = ref(0);

    setInterval(() => obj.value++, 2000);

    watch(obj, (valor, anterior) => {
      console.log(valor, anterior);
    });

    return {
      obj,
    };
  },
};
</script>
