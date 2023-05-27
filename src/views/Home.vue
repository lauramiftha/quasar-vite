<template>
    <q-page>
      <q-page-container>
        <h1>Welcome to Home Page</h1>
        <div>
          <router-link to="/about">Go to About Page</router-link>
        </div>
  
        <!-- Contoh layout tambahan -->
        <div class="layout">
          <h2>Layout 1</h2>
          <p>Ini adalah layout 1</p>
        </div>
  
        <div class="layout">
          <h2>Layout 2</h2>
          <p>Ini adalah layout 2</p>
        </div>
      </q-page-container>
    </q-page>
  </template>
  
  <script>
  export default {
    name: "Home",
  };
  </script>
  
  <style scoped>
  .layout {
    margin: 20px;
    padding: 10px;
    border: 1px solid #ccc;
  }
  </style>
  
