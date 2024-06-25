<template>
    <div class="layout">
        <NavBar />
        <main class="layout-content">
            <slot />
        </main>
        <Footer />
    </div>
</template>

<script setup>
import Footer from "@/components/footer/Footer.vue";
import NavBar from "@/components/navbar/NavBar.vue";
</script>

<style lang="scss" scoped>
.layout {
    .layout-content {
        min-height: 100vh;
        padding-top: 80px;
    }
}
</style>