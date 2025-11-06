<!-- src/components/OlaMundo.vue -->
<template>
  <h1>{{ mensagem }}</h1>
</template>

<script setup>
import { ref } from 'vue'

const mensagem = ref('Olá, Mundo!')
</script>

<style scoped>
h1 {
  color: #42b983;
  text-align: center;
}
</style>