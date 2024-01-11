<template>
  <div class="container container--xl">
    <p>e já fiz alguns projetos...</p>
    <div>
      <v-carousel
        height="170"
        :show-arrows="false"
        class="text-left"
        cycle
        hide-delimiters
        touch
      >
        <CardProject
          v-for="(project, index) in projects"
          :key="index"
          v-bind="project"
        />
      </v-carousel>
    </div>
  </div>
</template>

<script setup lang="ts">
const projects = [
  {
    title: "Portfólio",
    subtitle: "Vue.js 3 + Vuetify",
    text: "O site no quak você está agora",
    repoLink: "https://github.com/powerclonic/mdresch.com.br",
    siteLink: "https://mdresch.com.br",
  },
];
</script>

<style scoped>
@import url("@/assets/container.css");

.card {
  padding: 0px 10px;
}
</style>
