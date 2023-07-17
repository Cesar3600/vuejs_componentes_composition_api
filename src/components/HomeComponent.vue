<template>
  <div>{{ MyObj }}</div>
</template>

<script>
import { watch, ref } from "vue";
export default {
  setup() {
    const MyObj = ref(0);

    setInterval(() => MyObj.value++, 2000);

    watch(
      () => MyObj.value,
      (valor, anterior) => {
        console.log(valor, anterior);
      }
    );

    return {
      MyObj,
    };
  },
};
</script>
