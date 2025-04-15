<script setup>
import Hero from './components/Hero.vue';
import Social from './components/Social.vue';
import Projects from './components/Projects.vue';
import Posts from './components/Posts.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <main class="h-lvh">
    <div class="px-6 py-[8vh] max-w-[76ch] mx-auto xl:text-lg dark:prose-invert">
      <Profile></Profile>
      <Hero></Hero>
      <Social></Social>
      <Projects></Projects>
      <Posts></Posts>
      <Footer></Footer>
    </div>
  </main>
</template>

<style scoped></style>
