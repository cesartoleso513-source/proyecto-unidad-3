<template>
  <div class="space-y-8">
    <h2 class="text-4xl font-bold text-gray-800">Proyecto Unidad 3</h2>

    <p class="text-lg text-gray-600">
      Este proyecto demuestra el uso de directivas fundamentales en Vue 3.
    </p>

    <div class="grid md:grid-cols-2 gap-6">
      <div class="bg-blue-100 p-6 rounded-2xl shadow-lg hover:scale-105 transition">
        <h3 class="text-2xl font-semibold mb-2">v-if</h3>
        <p>Renderiza elementos condicionalmente en el DOM.</p>
      </div>

      <div class="bg-green-100 p-6 rounded-2xl shadow-lg hover:scale-105 transition">
        <h3 class="text-2xl font-semibold mb-2">v-show</h3>
        <p>Controla visibilidad mediante CSS.</p>
      </div>

      <div class="bg-yellow-100 p-6 rounded-2xl shadow-lg hover:scale-105 transition">
        <h3 class="text-2xl font-semibold mb-2">v-for</h3>
        <p>Permite iterar sobre listas dinámicamente.</p>
      </div>

      <div class="bg-purple-100 p-6 rounded-2xl shadow-lg hover:scale-105 transition">
        <h3 class="text-2xl font-semibold mb-2">v-bind:key</h3>
        <p>Optimiza el renderizado de listas en Vue.</p>
      </div>
    </div>
  </div>
</template>
