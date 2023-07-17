<template>
  <h2>{{ fullName }}</h2>
</template>

<script>
import { ref, computed } from "vue";
export default {
  setup() {
    const firstName = ref("Catherine");
    const lastName = ref("Alva");

    const fullName = computed(() => {
      return `${firstName.value} ${lastName.value}`;
    });

    return {
      fullName,
    };
  },
};
</script>
