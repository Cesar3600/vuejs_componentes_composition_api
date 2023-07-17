<template>
  <div>{{ obj.num }}</div>
</template>

<script>
import { watch, reactive } from "vue";
export default {
  setup() {
    const obj = reactive({ num: 0 });

    setInterval(() => obj.num++, 2000);

    watch(
      () => obj.num,
      (valor, anterior) => {
        console.log(valor, anterior);
      }
    );

    return {
      obj,
    };
  },
};
</script>
