<template>
  <div class="space-y-6">
    <h2 class="text-3xl font-bold text-purple-700">v-bind:key</h2>

    <p class="text-gray-600">La propiedad key ayuda a Vue a identificar elementos únicos.</p>

    <button
      @click="agregar"
      class="bg-purple-600 text-white px-6 py-2 rounded-lg hover:bg-purple-700 transition"
    >
      Agregar elemento
    </button>

    <ul class="space-y-3">
      <li v-for="item in lista" :key="item.id" class="bg-purple-100 p-4 rounded-lg shadow">
        🔹 {{ item.nombre }}
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const lista = ref([
  { id: 1, nombre: 'Elemento 1' },
  { id: 2, nombre: 'Elemento 2' },
])

let contador = 3

const agregar = () => {
  lista.value.push({
    id: contador++,
    nombre: `Elemento ${contador}`,
  })
}
</script>
