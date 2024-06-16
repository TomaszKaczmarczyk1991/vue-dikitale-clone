<template>
    <CountdownBar />
    <NavBar />
  </template>
  
  <script setup>
  import CountdownBar from '../components/CountdownBar.vue';
  import NavBar from '../components/NavBar.vue';
  </script>
  
  <style lang="scss" scoped>
  @import '../assets/styles/styles.scss';
  
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    // color: #2c3e50;
  }
  </style>