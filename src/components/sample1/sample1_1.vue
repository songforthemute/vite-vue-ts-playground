<template>
  <button @click="onClick">{{ item }}</button>
</template>

<script setup lang="ts">
let item = defineModel<number>({ default: 0 });

const onClick = () => {
  console.log("this is rendered", item.value++);
};
</script>

<style scoped></style>
