<script setup>
import Template from './base/模板语法/index.vue';
</script>

<template>
  <!-- 模板语法 -->
  <Template />
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: flex;
  min-height: 100vh;
  background-color: #f0f0f0;
  flex-direction: column;
  gap: 12px;
  align-items: center;
  justify-content: center;
}

.box {
  border: 1px solid #000;
  padding: 12px;
  border-radius: 4px;
  width: fit-content;
}
</style>
