<template>
  <div class="layout">
    <!-- Layout wrapper -->
    <main>
      <slot /> <!-- This will render your page content -->
    </main>
  </div>
</template>

<script setup>
// No imports needed unless you're using components
</script>

<style scoped>
.layout {
  background-color: #f8f9fa;
  min-height: 100vh;
  padding: 2rem;
}

main {
  max-width: 800px;
  margin: auto;
  background: white;
  padding: 2rem;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}
</style>
