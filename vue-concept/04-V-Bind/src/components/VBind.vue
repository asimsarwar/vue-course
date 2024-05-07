<script setup>
const vueUrl = 'https://vuejs.org/'
const amazingImage =
  'https://i.pinimg.com/736x/60/d7/1f/60d71f1b21e01427d4a0aedbebea0b94.jpg'
const altText = 'Just a random picture'

const imageWidth = 400
const imageHeight = 400
</script>

<template>
  <div>
    <!-- Old way 👇 -->
    <!-- <a v-bind:href="vueUrl">Vue Official Website</a> -->

    <!-- New way 👇 -->
    <a :href="vueUrl">Vue Official Website</a>
    <img :src="amazingImage" :alt="altText" :width="imageWidth" :height="imageHeight" />
  </div>
</template>
