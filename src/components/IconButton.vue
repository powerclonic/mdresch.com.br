<template>
  <button class="button">
    <img class="button__image" :src="iconFile" />
    <span class="button__text">{{ text }}</span>
  </button>
</template>

<script lang="ts" setup>
import * as icons from "@/assets/icons/index";

const props = defineProps({
  text: {
    type: String,
    required: true,
  },
  icon: {
    type: String,
    required: true,
  },
});

// @ts-expect-error
const iconFile = icons[props.icon];
</script>

<style scoped>
.button {
  background-color: rgb(var(--v-theme-secondary-darken-1));

  width: 100px;
  height: 35px;

  border-radius: 10px;
  color: rgb(var(--v-theme-primary));

  display: flex;
  flex-direction: column;
  align-items: center;
  overflow: hidden;
}

.button > * {
  margin: 2.5px;

  transition: 0.3s;
}
.button__image {
  height: 30px;
  aspect-ratio: 1/1;
}

.button:hover .button__image {
  margin-top: -32.5px;
}
</style>
