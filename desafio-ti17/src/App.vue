
<template>
  <Contador />
</template>
<script setup>
created: {
  document.oncontextmenu = document.body.oncontextmenu = function () {
    return false;
  };
}

import Contador from "./components/Contador.vue";
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
