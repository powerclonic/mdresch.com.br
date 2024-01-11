<template>
  <v-carousel-item class="item">
    <v-card rounded="10" height="170">
      <v-card-title>{{ title }}</v-card-title>
      <v-card-subtitle>{{ subtitle }}</v-card-subtitle>
      <v-card-text>{{ text }}</v-card-text>
      <v-card-actions>
        <v-btn variant="tonal" :href="repoLink" target="_blank"
          >Repositório</v-btn
        >
        <v-btn v-show="siteLink" :href="siteLink" target="_blank">Site</v-btn>
      </v-card-actions>
    </v-card>
  </v-carousel-item>
</template>

<script setup lang="ts">
defineProps({
  title: {
    type: String,
    required: true,
  },
  subtitle: {
    type: String,
    required: true,
  },
  text: {
    type: String,
    required: true,
  },
  repoLink: {
    type: String,
    required: true,
  },
  siteLink: {
    type: String,
    required: false,
  },
});
</script>
