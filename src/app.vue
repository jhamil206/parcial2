<script setup lang="ts">
import { storeToRefs } from 'pinia'
import { useProductoStore } from './stores/productoStore'

import LoginCard from './components/LoginCard.vue'
import AlmacenActivo from './components/AlmacenActivo.vue'

const store = useProductoStore()

const { estaLogueado } = storeToRefs(store)
</script>

<template>
  <div class="container mt-5">

    <LoginCard v-if="!estaLogueado" />

    <AlmacenActivo v-else />

  </div>
</template>