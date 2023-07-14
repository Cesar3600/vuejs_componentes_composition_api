<template>
  <h1>{{ user }} Repositories</h1>
</template>
<script>
export default {
  props: {
    user: {
      type: String,
      required: true,
    },
  },

  setup(props, ctx) {
    return {
      repositories,
    };
  },

  data() {
    return {
      repositories: [],
      filters: {},
      searchQuery: "",
    };
  },
  computed: {
    filteredRepositories() {
      return null;
    },
    repositoriesMatchingSearchQuery() {
      return null;
    },
  },
};
</script>
<style>
h1 {
  font-size: 33px;
}
</style>
