<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
        <RouterLink to="/products">Products</RouterLink>
      </nav>
    </div>
  </header>
  <RouterView />
</template>