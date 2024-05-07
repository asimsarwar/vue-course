<script setup>
const myMessage = 'Test Text Interpolation Module'
const myNumber = 100

function multiply(x, y) {
  return x * y
}
</script>

<template>
  <div>
    <h1>{{ myMessage }}</h1>
    <h1>{{ myNumber }}</h1>
    <h1>2 + 2 = {{ 2 + 2 }}</h1>
    <h1>Multiply Two Numbers: {{ multiply(3, 2) }}</h1>
    <!-- <p>Not allowed: {{ const myMessage = 'Testing..' }}</p> ❌ -->
  </div>
</template>
