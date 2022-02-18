<script setup>
import "mind-ar/dist/mindar-image.prod.js";
import "aframe";
import "mind-ar/dist/mindar-image-aframe.prod.js";
import "mind-ar/dist/mindar-face.prod.js";
import "mind-ar/dist/mindar-face-aframe.prod.js";
import "mind-ar/dist/mindar-face-three.prod.js";

import MindarViewer from "./components/MindarViewer.vue";
import { ref } from "vue";

const mindarViewerRef = ref(null);
</script>

<template>
  <div class="app">
    <h1>
      Vue 3 com
      <a href="https://github.com/hiukim/mind-ar-js" target="_blank">MindAR</a>
    </h1>

    <div class="container">
      <mindar-viewer ref="mindarViewerRef" />
    </div>
  </div>
</template>

<style scoped>
.app {
  text-align: center;
}

.container {
  margin: 20px auto;
  position: relative;
  height: 400px;
  width: 600px;
  overflow: hidden;
}
</style>
