<template>
  <h2>{{ fullName }}</h2>
</template>

<script>
import { toRefs, computed } from "vue";

export default {
  props: {
    firstName: {
      type: String,
    },
    lastName: {
      type: String,
    },
  },
  setup(props) {
    const { firstName, lastName } = toRefs(props);

    const fullName = computed(() => {
      return `${firstName.value} ${lastName.value}`;
    });

    return {
      fullName,
    };
  },
};
</script>
