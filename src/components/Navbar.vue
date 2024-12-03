<script setup>

  import { RouterLink } from 'vue-router';

</script>

<template>
  
  <nav class="navbar-container">
    <ul class="navbar-items">
      <router-link to="/" class="navabr-item">INICIO</router-link>
      <router-link to="/about" class="navabr-item">ABOUT ME</router-link>
      <li class="navabr-item">SERVICES</li>
      <li class="navabr-item">PROJECTS</li>
      <li class="navabr-item">CONTACT US</li>
    </ul>
  </nav>

</template>

<style scoped>
  
  .navbar-container {
    display: flex;
    background-color: #000;
    margin: 0 auto;
  }
  .navbar-items {
    display: flex;
    flex-direction: row;
    justify-content: flex-end;
    padding-right: 20px;
    color: #fff;
  }

</style>
