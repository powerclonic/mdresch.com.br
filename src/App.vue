<template>
  <v-app>
    <v-main>
      <TheHeader />
      <article class="content">
        <TheResume />
        <TheStack />
        <TheLanguages />
        <TheSocials />
        <TheFooter />
      </article>
    </v-main>
  </v-app>
</template>

<script setup lang="ts">
//
</script>

<style>
body {
  font-family: "Fredoka", Arial, Helvetica, sans-serif;
}

.content {
  padding: 10px;
  display: flex;
  flex-direction: column;
  gap: 20px;
}
</style>
