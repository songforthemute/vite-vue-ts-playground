<template>
  <form action="" @submit.prevent="submitForm">
    <div>
      <label for="userId">ID: </label>
      <input type="text" id="userId" v-model="username">
    </div>
    <div>
      <label for="password">PW: </label>
      <input type="password" id="password" v-model="password">
    </div>
    <button type="submit">로그인</button>
  </form>
</template>

<script lang="ts">
import axios from "axios";

export default {
  data() {
    return {
      username: '',
      password: '',
    }
  },methods: {
    submitForm() {
      const data = {
        username: this.username,
        password: this.password,
      }

      axios.post("https://jsonplaceholder.typicode.com/users/", data).then((res) => {
        console.log(res)
      })
    }
  }
}
</script>

<style scoped>

</style>