<script setup>
import { provide } from 'vue'
import SchoolComponent from './SchoolComponent.vue'

provide('studentName', 'Alex')
provide('studentAge', 20)
provide('studentLocation', ['Earth', 'IDK'])
</script>

<template>
  <SchoolComponent />
</template>
