<script setup>
 
  import { RouterView, RouterLink } from 'vue-router';
  import { useDark, useToggle } from '@vueuse/core';

  import DarkModeButton from './components/DarkModeButton.vue';

  /*const isDark = useDark({
    selector: 'body',
    attribute: 'class', 
    valueDark: 'dark',
    valueLight: '',
  });
  const toggleDark = useToggle(isDark);
*/
</script>

<template>
  
  <nav class="navbar-container">
    
    <div class="logo-container">
      <span>logo</span>
    </div>
    
    <div class="navbar-items">
      <router-link to="/" class="navbar-item">HOME</router-link>
      <router-link to="/about" class="navbar-item">ABOUT ME</router-link>
      <router-link to="/services" class="navbar-item">SERVICES</router-link>
      <router-link to="/projects" class="navbar-item">PROJECTS</router-link>
      <router-link to="/contact" class="navbar-item">CONTACT US</router-link>
    </div>

    <div class="actions-button">
      
      <DarkModeButton/>
      <i id="bars-icon" class="fa-solid fa-bars"></i>
      
    </div>
  
  </nav>

  <main class="main-container">
  
    <RouterView />
  
  </main>

</template>

<style>
  
  * {
    margin: 0px;
    font-family: "Roboto Mono", monospace; 
  }
  
  body.dark .navbar-container {
    background-color: #000;
    color: #fff;
  } 

  .navbar-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 20px;
    padding-bottom: 20px;
    padding-left: 20px;
    padding-right: 20px;
  }
  .navbar-container.dark {
    background-color: #000;
    color: #fff;
  } 

  .navbar-items {
    display: flex;
    justify-content: center;
    gap: 10px;
  
  }
  .navbar-item {
    text-decoration: none;
    font-weight: bold;
    font-size: 20px;
    color: #000;
  }
  body.dark .navbar-item {
    color: #fff;
  }

  .actions-button {
    display: flex;
    gap: 10px;
    align-items: center;
  }
  .#dark-btn {
    max-width: 50px;
    max-height: 5px;
  }
  .actions-button i {
    cursor: pointer;
  }

  @media (max-width: 768px) {
    .navbar-items {
      display: none;
    }
  }

</style>
