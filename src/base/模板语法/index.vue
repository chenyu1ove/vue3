<template>
  <div class="box">
    <h1>模板语法</h1>
    <!-- 文本插值 -->
    <div class="box">
      <h2>文本插值</h2>
      <div>{{ 'Hello, Vue 3!' }}</div>
      <div>{{ 5 + 3 }}</div>
    </div>
    <!-- 原始html -->
    <div class="box">
      <h2>原始 HTML</h2>
      <div v-html="'<strong style=color:red>这是加粗的红色文本</strong>'"></div>
    </div>
    <!-- 属性绑定 响应式地绑定一个 attribute -->
    <div class="box">
      <h2>属性绑定</h2>
      <!-- :src="'https://vuejs.org/images/logo.png'" -->
      <img
        v-bind:src="'https://vuejs.org/images/logo.png'"
        alt="Vue Logo"
        width="100"
      />
      <div v-bind="objectOfAttrs">动态绑定多个值</div>
      <form v-on:submit="onSubmit"><button type="submit">提交</button></form>
    </div>
  </div>
</template>

<script setup>
const objectOfAttrs = {
  id: 'container',
  class: 'wrapper',
  style: 'background-color:green',
};
const onSubmit = (event) => {
  event.preventDefault();
  alert('表单已提交！');
};
</script>
