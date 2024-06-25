<template>
    <Layout>
      <Hero />
    </Layout>
</template>
  
  <script setup>
  import Layout from '../layout/Layout.vue';
  import Hero from '../components/Hero.vue';

  </script>
  
  <style lang="scss" scoped>
  @import '../assets/styles/styles.scss';
  
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
  }
  </style>