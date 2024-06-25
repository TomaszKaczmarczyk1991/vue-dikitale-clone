<template>
    <div class="hero-container">
      <img alt="hero" src="../assets/styles/img/logo/hero-1248-2x.webp"/>
      <div class="text">
        <h3>
        The SME forum <br> for
        <span class="blue-highlight">Digitalisation & AI</span>
      </h3>
      </div>
    </div>
  </template>
  
<style lang="scss" scoped>
@import '/src/assets/styles/styles.scss';
  .hero-container {
    text-align: center;
    padding-top: 100px;
    width: 100%;
    height: 100vh;
    
  }
  
  img {
    max-width: 100%;
    height: auto;
  }

  .text {
    position: absolute;
    font-size: 48px;
    font-weight: 400;
    line-height: 56px;
    font-family: Roboto, sans-serif;
    top: 80%;
    left: 20%;
    transform: translate(-50%, -50%);
    text-align: left;
  }

  .blue-highlight {
    color: $blue-text
  }
  </style>
  