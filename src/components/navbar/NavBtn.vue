<template>
    <div class="btn-container">
      <button 
        class="nav-btn" 
        v-for="(button, index) in buttons"
        :key="index"
      >
        {{ button.label }}
      </button>
    </div>
  </template>
  
  <script setup>
  const buttons = [
    { label: 'Home' },
    { label: 'General Information' },
    { label: 'Exhibitor' },
    { label: 'Specialist Program' },
    { label: 'Advisory Board' },
    { label: 'Request Stand' },
  ];
  </script>
  
  <style lang="scss" scoped>
  @import '/src/assets/styles/_variables.scss';
  
  .btn-container{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 80px;
    margin-top: 20px;
  
    .nav-btn {
      height: 36px;
      padding: 5px 10px;
      background-color: $countdown-background;
      color: white;
      border: none;
      border-radius: 16px;
      cursor: pointer;
      margin: 5px;
    }
}
  </style>

<!-- TO DO:
- highlight button when active
- add scroll function onClick
-->