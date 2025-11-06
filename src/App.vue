<!-- src/App.vue -->
<template>
  <div class="container">
    <h1>Exibição Condicional</h1>

    <Mensagem v-if="mostrar" />
    <p v-else>Nenhuma mensagem disponível.</p>
    <button @click="mostrar = !mostrar">
      Alternar Exibição
    </button>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import Mensagem from './components/Mensagem.vue'

const mostrar = ref(true)
</script>