<template>
    <q-page>
      <q-page-container>
        <h1>About Page</h1>
        <p>This is the about page of our application.</p>
  
        <!-- Contoh layout tambahan -->
        <div class="layout">
          <h2>About Layout 1</h2>
          <p>Ini adalah layout menarik untuk halaman About</p>
          <q-img
            src="/path/to/image.jpg"
            alt="About Image"
            class="about-image"
          />
        </div>
  
        <div class="layout">
          <h2>About Layout 2</h2>
          <p>Ini adalah layout lain yang menarik untuk halaman About</p>
          <q-img
            src="/path/to/another-image.jpg"
            alt="Another About Image"
            class="about-image"
          />
        </div>
      </q-page-container>
    </q-page>
  </template>
  
  <script>
  export default {
    name: "About",
  };
  </script>
  
  <style scoped>
  .layout {
    margin: 20px;
    padding: 10px;
    border: 1px solid #ccc;
  }
  
  .about-image {
    width: 200px;
    height: auto;
    margin-top: 10px;
  }
  </style>
  
