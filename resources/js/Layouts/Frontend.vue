<template>
  <div class="bg-slate-200 dark:bg-slate-900">
    <Header />
    <!-- header -->
    <main class="min-h-screen md:pt-[90px]">
      <slot />
    </main>
    <Footer />
  </div>
</template>

<script setup>
import Header from "@/Components/Frontend/Header.vue";
import Footer from "@/Components/Frontend/Footer.vue";
</script>

<style></style>
