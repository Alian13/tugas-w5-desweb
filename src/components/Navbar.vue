<script setup>
import { RouterLink, useRoute } from "vue-router";

const route = useRoute();
const active = (name) =>
  route.name === name
    ? "text-blue-600 font-semibold"
    : "text-gray-700 hover:text-blue-500";
</script>

<template>
  <nav class="bg-white shadow-sm sticky top-0 z-50">
    <div class="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center">
      <h1 class="text-xl font-bold text-blue-600">Kota Balikpapan</h1>

      <div class="space-x-6">
        <RouterLink class="text-gray-600 hover:text-blue-600" to="/"
          >Home</RouterLink
        >
        <RouterLink class="text-gray-600 hover:text-blue-600" to="/contact"
          >Contact</RouterLink
        >
      </div>
    </div>
  </nav>
</template>
