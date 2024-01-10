<template>
  <footer class="footer">
    <div class="footer__bar"></div>
    <div class="pa-4">
      <h3 class="footer__title">MATHEUS DRESCH</h3>
      <p class="footer_year">2024</p>
    </div>
  </footer>
</template>

<style scoped>
.footer__title {
  font-family: "Fredoka", Arial, Helvetica, sans-serif;
  font-size: 1.75rem;

  text-align: center;
}

.footer__bar {
  width: 100%;
  height: 5px;
  background-color: rgb(var(--v-theme-primary));
  box-shadow: 0px -4px 4px 0px rgba(245, 110, 15, 0.25);
}

.footer_year {
  text-align: center;
  font-weight: bold;
}
</style>
