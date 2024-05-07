<script setup>
import { ref } from 'vue'
const username = ref('')
const email = ref('')
const password = ref('')
</script>

<template>
  <form @submit.prevent="$emit('userInfo', username, email, password)">
    <input type="text" v-model="username" />
    <input type="email" v-model="email" />
    <input type="password" v-model="password" />
    <button type="submit">Submit</button>

    <h4>UserName: {{ username }}</h4>
    <h4>Email: {{ email }}</h4>
    <h4>Password: {{ password }}</h4>
  </form>
</template>
