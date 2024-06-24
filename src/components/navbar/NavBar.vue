<template>
    <header class="header">
        <nav class="navbar">
            <img alt="logo" src="/src/assets/styles/img/logo/logo-nav-768-2x.webp">
        </nav>
        <CountdownBar />
    </header>
</template>

<script setup>
import CountdownBar from '@/components/CountdownBar.vue';
</script>

<style lang="scss" scoped>
@import '/src/assets/styles/styles.scss';
.header {
    //left: 0;
    position: fixed;
    top: 0;
    width: 100vw;

    .navbar {
        background-color: $navbar-background;
    }

}
</style>