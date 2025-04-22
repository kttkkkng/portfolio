<script setup>
import WorkExperience from './sections/WorkExperience.vue'
import Skill from './sections/Skill.vue'
</script>

<template>
  <header class="fixed z-10 flex justify-between items-center bg-white shadow-md p-6 w-full h-20">
    <p class="text-[24px]">Teerawat</p>
  </header>
  <div class="header-padding"></div>
  <section id="home" class="fade-in grid grid-rows-[min-content,1fr]">
    <p class="text-[70px]">Welcome.</p>
    <p class="text-[30px]">My name is <span class="text-green-500">Teerawat Tattananurat</span>. I'm a <span class="text-green-500">fullstack developer</span> based in Bangkok. I have many years of experience in <span class="text-green-500">Django</span>, <span class="text-green-500">Vue.js</span> and <span class="text-green-500">Node.js</span>. However, I'm also open to learn new technology as well.</p>
  </section>
  <WorkExperience/>
  <Skill/>
  <section id="contact" class="fade-in">
    <p class="text-[40px]">Contact Me</p>
    <div class="grid grid-cols-[2rem,1fr] items-center gap-4 mt-4">
      <img src="./assets/phone.png" class="w-8 h-8" /><p class="text-[24px]">082-504-7971</p>
      <img src="./assets/email.png" class="w-8 h-8" /><p class="text-[24px]">teerawat7971@gmail.com</p>
    </div>
  </section>
</template>

<style>
.header-padding {
  height: 80px;
}

@keyframes fadeIn {
  to { opacity: 1; }
}

section {
  padding: 12rem 2.5rem;
  max-width: 1000px;
  margin: 0 auto;
}

@media (prefers-reduced-motion: no-preference) {
  @supports (animation-timeline: scroll()) {
    .fade-in {
      opacity: 0;
      animation: fadeIn ease-in forwards;
      animation-timeline: view();
      animation-range: entry 200px 500px;
    }
  }
}
</style>
