<template>
  <div class="space-y-6">
    <h2 class="text-3xl font-bold text-blue-700">Directiva v-if</h2>

    <p class="text-gray-600">v-if renderiza o elimina completamente el elemento del DOM.</p>

    <button
      @click="mostrar = !mostrar"
      class="bg-blue-600 text-white px-6 py-2 rounded-lg hover:bg-blue-700 transition"
    >
      {{ mostrar ? 'Ocultar mensaje' : 'Mostrar mensaje' }}
    </button>

    <div v-if="mostrar" class="p-6 bg-blue-100 rounded-xl shadow-lg border-l-4 border-blue-600">
      Este mensaje existe en el DOM solo cuando la condición es verdadera.
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
const mostrar = ref(false)
</script>
