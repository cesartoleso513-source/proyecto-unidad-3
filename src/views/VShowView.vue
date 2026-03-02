<template>
  <div class="space-y-6">
    <h2 class="text-3xl font-bold text-green-700">Directiva v-show</h2>

    <p class="text-gray-600">v-show solo cambia la visibilidad usando CSS (display: none).</p>

    <button
      @click="visible = !visible"
      class="bg-green-600 text-white px-6 py-2 rounded-lg hover:bg-green-700 transition"
    >
      {{ visible ? 'Ocultar' : 'Mostrar' }}
    </button>

    <div v-show="visible" class="p-6 bg-green-100 rounded-xl shadow-lg border-l-4 border-green-600">
      Este mensaje siempre está en el DOM, solo se oculta visualmente.
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
const visible = ref(true)
</script>
