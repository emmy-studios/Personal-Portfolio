<script setup>

  import { RouterLink } from 'vue-router';

</script>

<template>
  
  <nav class="navbar-container">
    <ul class="navbar-items">
      <router-link to="/" class="navbar-item">HOME</router-link>
      <router-link to="/about" class="navbar-item">ABOUT ME</router-link>
      <router-link to="/services" class="navbar-item">SERVICES</router-link>
      <router-link to="/projects" class="navbar-item">PROJECTS</router-link>
      <router-link to="/contact" class="navbar-item">CONTACT US</router-link>
    </ul>
  </nav>

</template>

<style scoped>
  
  .navbar-container { 
    display: flex;
    flex-direction: column;
    background-color: #000;
  }
  .navbar-items {
    display: flex;
    justify-content: flex-end;
    gap: 20px;
    color: #fff;
  }
  .navbar-item {
    text-decoration: none;
    color: #fff;
  }

</style>
