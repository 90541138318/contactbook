<script setup>
import { computed } from 'vue'
import { useRoute } from 'vue-router'

import DefaultLayout from './layouts/DefaultLayout.vue'
import AdminLayout from './layouts/AdminLayout.vue'

const route = useRoute()

const layout = computed(() => {
  if (route.path.startsWith('/edit')) return AdminLayout
  return DefaultLayout
})
</script>

<template>
  <component :is="layout">
    <router-view />
  </component>
</template>
