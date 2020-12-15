<template>
  <b-container>
    <h2>Projects</h2>
    <b-card-group columns class="d-flex justify-content-center flex-wrap">
      <b-card
        v-for="project in projects"
        :key="project.name"
        :title="project.name"
        class="mx-1"
      >
        {{ project.description }}
      </b-card>
    </b-card-group>
  </b-container>
</template>

<script>
export default {
  data: function () {
    return {
      projects: [
        {
          name: "Music Analyzer",
          description:
            "Created a program in Java to analyze musical artists and their songs and output relationship data to the user.",
        },
        {
          name: "Residence Hall Manager",
          description:
            "Created an application in Java to track student information for Purdue residence halls.",
        },
      ],
    };
  },
};
</script>

<style scoped>
.card {
  max-width: 20em;
}
</style>
