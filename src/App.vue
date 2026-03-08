<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <nav>
      <RouterLink to="/">首页</RouterLink>
      <RouterLink to="/about">关于</RouterLink>
    </nav>
  </header>
  <RouterView />
</template>

<style scoped>
header {
  padding: 1rem;
  background-color: #f5f5f5;
}

nav {
  display: flex;
  gap: 1rem;
}

nav a {
  color: #333;
  text-decoration: none;
}

nav a:hover {
  color: #409eff;
}

nav a.router-link-active {
  color: #409eff;
  font-weight: bold;
}
</style>
