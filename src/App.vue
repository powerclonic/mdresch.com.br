<template>
  <v-app>
    <v-main>
      <div class="container">
        <TheHeader />
        <article class="content">
          <TheResume />
          <TheStack />
          <TheLanguages />
          <TheProjects class="div1" />
          <TheMessage class="div2" />
          <TheSocials />
        </article>
        <TheFooter />
      </div>
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

.container {
  display: flex;
  flex-direction: column;

  justify-content: space-between;

  height: 100%;
}
.content {
  padding: 10px;
  display: flex;
  flex-direction: column;
  gap: 20px;
}

@media screen and (min-width: 769px) {
  .content {
    padding: 32px 12.5vw;

    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(4, 1fr);
    grid-column-gap: 20px;
    grid-row-gap: 20px;
  }

  .div1 {
    grid-area: 2 / 2 / 4 / 3;
  }
  .div2 {
    grid-area: 3 / 1 / 5 / 2;
  }
}
</style>
