<template>
  <div class="min-h-screen bg-gray-100">
    <!-- Header -->
    <header class="bg-blue-600 text-white p-6 shadow-lg">
      <h1 class="text-3xl font-bold text-center">Proyecto Unidad 3 🚀</h1>
    </header>

    <!-- Navegación -->
    <nav class="bg-white shadow-md p-4 flex justify-center gap-6 text-lg font-medium">
      <router-link class="hover:text-blue-600 transition" to="/">Inicio</router-link>
      <router-link class="hover:text-blue-600 transition" to="/v-if">v-if</router-link>
      <router-link class="hover:text-blue-600 transition" to="/v-show">v-show</router-link>
      <router-link class="hover:text-blue-600 transition" to="/v-for">v-for</router-link>
      <router-link class="hover:text-blue-600 transition" to="/v-key">v-bind:key</router-link>
    </nav>

    <!-- Contenido -->
    <main class="p-8 max-w-4xl mx-auto">
      <div class="bg-white p-6 rounded-xl shadow-lg">
        <router-view />
      </div>
    </main>
  </div>
</template>
