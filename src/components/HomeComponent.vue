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
  setup(props, { expose }) {
    const { firstName, lastName } = toRefs(props);

    const fullName = computed(() => {
      return `${firstName.value} ${lastName.value}`;
    });
    //console.log(context);

    expose({
      fullName,
    });

    return {
      fullName,
    };
  },
};
</script>
