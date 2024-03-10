<template>
  <Sample2Header :appTitle="msg" @change="changeMessage" />
  <button @click="showAlert">경고</button>
</template>

<script lang="ts">
import Sample2Header from "./Sample2-header.vue";

  export default {
    components: {
      Sample2Header,
    }
    ,data() {
      return {
        msg: '앱 헤더 컴포넌트'
      }
    },
    methods: {
      showAlert() {
        alert('hello!')
      },
      changeMessage() {
        this.msg = '변경 완료'
      }
    }
}
</script>


<style scoped>

</style>