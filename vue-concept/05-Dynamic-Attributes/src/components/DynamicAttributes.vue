<script setup>
// Dynamic Binding With Multiple Attributes
const imageInfo = {
  src: 'https://i.pinimg.com/736x/60/d7/1f/60d71f1b21e01427d4a0aedbebea0b94.jpg',
  alt: 'Just a random picture',
  width: 400,
  height: 400
}
</script>

<template>
  <div>
    <!-- <img v-bind="imageInfo" /> -->
    <img :="imageInfo" />
  </div>
</template>
