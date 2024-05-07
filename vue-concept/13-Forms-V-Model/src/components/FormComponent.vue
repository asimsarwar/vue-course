<script setup>
import { reactive } from 'vue'
const formData = reactive({ username: '', email: '', password: '' })
const submitHandler = (e) => {
  e.preventDefault()
  alert('Form has been submitted!')
}
</script>

<template>
  <!-- One Way -->
    <!-- <form @submit.prevent="alert('Form has been submitted!')"> -->
  <!-- Second Way -->    
    <!-- <form @submit="submitHandler"> -->
  <!-- Third Way -->  
  <form v-on:submit="submitHandler">
    <input type="text" placeholder="Please enter your name." v-model="formData.username" />
    <input type="email" placeholder="Please enter your email." v-model="formData.email" />
    <input type="password" placeholder="Please enter your password." v-model="formData.password" />
    <button type="submit">Submit</button>
  </form>

  <h1>{{ formData.username }}</h1>
  <h1>{{ formData.email }}</h1>
  <h1>{{ formData.password }}</h1>
</template>
