<template>
  <b-container>
    <b-button
      v-for="link in links"
      :key="link.name"
      :href="link.url"
      variant="primary"
      class="mx-1"
    >
      {{ link.name }}
    </b-button>
  </b-container>
</template>

<script>
export default {
  data: function () {
    return {
      links: [
        {
          name: "GitHub",
          url: "https://github.com/weekofcode24",
        },
        {
          name: "LinkedIn",
          url: "https://linkedin.com",
        },
      ],
    };
  },
};
</script>

<style scoped>
</style>
