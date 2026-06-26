<script setup lang="ts">
import { ref } from 'vue';

// 1. CONTRATOS DE TIPADO
interface Producto {
  id: number;
  nombre: string;
  precio: number;
  stock: number;
  imagen: string;
}

// 2. ESTADO REACTIVO e INTERFACES
const isAuthenticated = ref(false);
// ... Tus variables y funciones del laboratorio (handleLogin, etc.)
</script>

<template>
  <div class="container mt-5">
    <div v-if="!isAuthenticated">
      </div>
    <div v-else>
      </div>
  </div>
</template>

<style scoped>
/* Tus estilos personalizados */
</style>