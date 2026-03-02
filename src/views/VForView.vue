<template>
  <div class="space-y-6">
    <h2 class="text-3xl font-bold text-yellow-600">Directiva v-for</h2>

    <p class="text-gray-600">v-for permite renderizar listas dinámicamente.</p>

    <ul class="space-y-3">
      <li
        v-for="(fruta, index) in frutas"
        :key="index"
        class="bg-yellow-100 p-4 rounded-lg shadow hover:scale-105 transition"
      >
        {{ fruta }}
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts">
const frutas = ['Manzana', 'Plátano', 'Fresa', 'Uva']
</script>
