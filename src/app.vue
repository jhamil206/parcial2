<script setup lang="ts">
import LoginCard from './components/LoginCard.vue';
import AlmacenActivo from './components/AlmacenActivo.vue';
import { useProductoStore } from './stores/productoStore';

const store = useProductoStore();
</script>

<template>
  <main class="bg-light d-flex align-items-center justify-content-center w-100" style="min-height: 100vh;">
    <div class="w-100" style="padding: 20px;">
      <LoginCard v-if="!store.estaLogueado" />
      <AlmacenActivo v-else />
    </div>
  </main>
</template>