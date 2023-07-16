<template>
  <div>{{ MyObj.counter }}</div>
</template>

<script>
import { reactive } from "vue";
export default {
  setup() {
    const MyObj = reactive({ counter: 0 });

    setInterval(() => MyObj.counter++, 500);

    return {
      MyObj,
    };
  },
};
</script>
