<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <nav class="navbar bg-body-tertiary">
    <div class="container-fluid">
      <div>
      <RouterLink to="/">Home</RouterLink> |
      <RouterLink to="/register">Register</RouterLink> |
      <RouterLink to="/login">Login</RouterLink>
      </div>
      
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-primary" type="submit">Search</button>
      </form>
      
      <div>
        <a href="/login" class="btn btn-primary me-2" type="button">Login</a>
        <a href="/register" class="btn btn-primary me-2" type="button">Create an account</a>
      </div>
    </div>
  </nav>

  <RouterView />
</template>