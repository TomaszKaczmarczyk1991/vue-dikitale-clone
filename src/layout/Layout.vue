<template>
    <div class="layout">
        <NavBar />
        <main class="layout-content">
            <slot />
            <Hero />
        </main>
        <Footer />
    </div>
</template>

<script setup>
import Footer from "@/components/footer/Footer.vue";
import NavBar from "@/components/navbar/NavBar.vue";
import Hero from "@/components/Hero.vue";
</script>

<style lang="scss" scoped>
.layout {
    .layout-content {
        min-height: 100vh;
        padding-top: 80px;
    }
}
</style>