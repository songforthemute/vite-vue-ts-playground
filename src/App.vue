<script setup lang="ts">
import HelloWorld from "./components/HelloWorld.vue";
import Sample from "./components/sample.vue";
import Sample1 from "./components/sample1.vue";
import Sample2 from "./components/Sample2.vue";
import Main from "./components/toy/Main.vue";
</script>

<template>
  <!--  <div>-->
  <!--    <a href="https://vitejs.dev" target="_blank">-->
  <!--      <img src="/vite.svg" class="logo" alt="Vite logo" />-->
  <!--    </a>-->
  <!--    <a href="https://vuejs.org/" target="_blank">-->
  <!--      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />-->
  <!--    </a>-->
  <!--  </div>-->
  <!--  <Sample/>-->
<!--  <Sample1 />-->
<!--  <Sample2/>-->
  <Main/>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
