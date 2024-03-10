<template>
  <div v-if="showing">
    <div v-for="data in obj.data.data" :key="data.item">
      <Sample1_1 v-model="data.item" />
    </div>
  </div>
  <button @click="showing = !showing">클릭</button>
</template>

<script setup lang="ts">
import { ref } from "vue";
import Sample1_1 from "./sample1/sample1_1.vue";

const obj = ref({
  id: 0,
  data: {
    id: 0,
    data: Array.from({ length: 10 }, (_, i) => ({ item: i + 1 })),
  },
});

const showing = ref(false);
</script>

<style scoped></style>
