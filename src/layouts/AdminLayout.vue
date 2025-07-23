<template>
  <div class="admin-layout">
    <aside class="sidebar">
      <h2>Admin Sidebar</h2>
      <!-- Add sidebar navigation here -->
    </aside>

    <main class="content">
      <slot /> <!-- This is where page content will go -->
    </main>
  </div>
</template>

<script setup>
// No script is needed unless you want interactivity
</script>

<style scoped>
.admin-layout {
  display: flex;
  height: 100vh;
}

.sidebar {
  width: 250px;
  background-color: #2c3e50;
  color: white;
  padding: 1rem;
}

.content {
  flex: 1;
  padding: 2rem;
  background-color: #f8f8f8;
}
</style>
