<template>
 <h1>{{ appTitle }}</h1>
  <button @click="changeTitle">바꾸기</button>
</template>

<script lang="ts">
export default {
  props: ['appTitle']
  ,methods: {
    changeTitle() {
      this.$emit('change')
    }
  }
}
</script>

<style scoped>

</style>