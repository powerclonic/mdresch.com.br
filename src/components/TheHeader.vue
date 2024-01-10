<template>
  <header class="header">
    <h1 class="header__title">dresch</h1>
    <div class="header__bar"></div>
  </header>
</template>

<style scoped>
.header__title {
  font-family: "Fredoka", Arial, Helvetica, sans-serif;
  font-size: 3rem;

  text-align: center;
}

.header__bar {
  width: 100%;
  height: 5px;
  background-color: rgb(var(--v-theme-primary));
  box-shadow: 0px 4px 4px 0px rgba(245, 110, 15, 0.25);
}
</style>
