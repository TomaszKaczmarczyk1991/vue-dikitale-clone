<template>
    <header class="header">
        <CountdownBar />
        <nav class="navbar">
            <img class="img" alt="logo" src="../../assets/styles/img/logo/logo-nav-768-2x.webp">
            <NavBtn />
        </nav>
    </header>
</template>

<script setup>
import CountdownBar from '@/components/CountdownBar.vue';
import NavBtn from '@/components/navbar/NavBtn.vue';
</script>

<style lang="scss" scoped>
@import '/src/assets/styles/styles.scss';

.header {
    left: 0;
    position: fixed;
    top: 0;
    width: 100vw;

    .navbar {
        background-color: $navbar-background;
        height: 176px;

    }
    
    .img {
        display: block;
        position: relative;
        top: 6rem;
        height: auto;
        max-width: 40%;
        max-height: 40%;
        padding-left: 160px;
    }
}
</style>