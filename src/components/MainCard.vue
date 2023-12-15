<template>
    <div id="app">
      <section class="section" id="section1">
        <div class="content">
        </div>
      </section>
      <section class="section" id="section2">
        <div class="content">
        </div>
      </section>
      <section class="section" id="section3">
        <div class="content">
        </div>
      </section>
    </div>
  </template>
  
  <script>
  export default {
    name: 'App',
  };
  </script>
  
  <style>
  body {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  #app {
    display: flex;
  }
  
  .section {
    flex: 1;
    overflow-y: auto;
    padding: 20px;
    border: 20px solid #ccc;
    margin: 10px;
  }
  
  .content {
  }
  </style>
  