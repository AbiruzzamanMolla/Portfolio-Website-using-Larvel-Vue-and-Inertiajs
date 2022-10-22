<script setup>
import { Head, Link } from "@inertiajs/inertia-vue3";
import FrontendLayout from "@/Layouts/Frontend.vue";
import Hero from "@/Components/Frontend/Hero.vue";
import About from "@/Components/Frontend/About.vue";
import Promotion from "@/Components/Frontend/Promotion.vue";
import Skills from "@/Components/Frontend/Skills.vue";
import Portfolio from "@/Components/Frontend/Portfolio.vue";
import Services from "@/Components/Frontend/Services.vue";
import Contact from "@/Components/Frontend/Contact.vue";

defineProps({
  skills: Object,
  projects: Object,
});
</script>

<template>
  <Head title="Welcome to Portfolio" />
  <FrontendLayout>
    <!-- hero section - primary -->
    <Hero />
    <!-- promote section - tail -100 -->
    <Promotion />
    <!-- about section secoundary color -->
    <About />
    <!-- skills sections tail - 100 -->
    <Skills :skills="skills" />
    <!-- portfolio primary -->
    <Portfolio :skills="skills" :projects="projects" />
    <!-- services secoundary -->
    <Services />
    <!-- contact section primary -->
    <Contact />
  </FrontendLayout>
</template>
