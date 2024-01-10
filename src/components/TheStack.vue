<template>
  <div class="container">
    <p>minha stack principal é...</p>
    <div class="buttons">
      <IconButton text="Vue.js" icon="vue" />
      <IconButton text="Laravel" icon="laravel" />
      <IconButton text="MySQL" icon="mysql" />
    </div>
  </div>
</template>

<style scoped>
@import url("@/assets/container.css");

.buttons {
  display: flex;
  justify-content: space-around;
}
</style>
