<script setup>
import Projects from "./Projects.vue";
defineProps({
  skills: Object,
  projects: Object,
});
</script>
<template>
  <section
    id="portfolio"
    class="section bg-light-primary dark:bg-dark-primary min-h-[1400px]"
  >
    <div class="container mx-auto">
      <div class="flex flex-col items-center text-center">
        <h2 class="section-title">My latest works</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Atque veniam debitis
          fuga officiis tempore temporibus odio nulla quos, distinctio eligendi
          perferendis accusantium facere dolore praesentium. Tenetur totam dicta repellat
          incidunt.
        </p>
      </div>
      <Projects :skills="skills" :projects="projects" />
    </div>
  </section>
</template>
