<script setup>
import Skills from "./components/Skills.vue";
import Projects from "./components/Projects.vue";
import About from "./components/About.vue";
import Home from "./components/Home.vue";

import { ref } from 'vue';
const skills = ref(null);
const projects = ref(null);
const about = ref(null);
const scrollToSkillsReference = () => {
  const targetSkills = skills.value?.$el || skills.value;
  if (targetSkills) {
    targetSkills.scrollIntoView({ behavior: 'smooth' });
  } else {
    console.error('No reference found');
  }
};
const scrollToProjectReference = () => {
  const targetProjects = projects.value?.$el || projects.value;
  if (targetProjects) {
    targetProjects.scrollIntoView({ behavior: 'smooth' });
  } else {
    console.error('No reference found');
  }
};
const scrollToAboutReference = () => {
  const targetAbout = about.value?.$el || about.value;
  if (targetAbout) {
    targetAbout.scrollIntoView({ behavior: 'smooth' });
  } else {
    console.error('No reference found');
  }
};
</script>

<template>
  <div>
    <header class="flex flex-col md:flex-row md:items-start p-4 md:p-8 lg:p-12">
      <div class="flex-none text-start mb-4 md:mb-0 md:mr-8">
        <a>coumba</a>
      </div>
      <div class="flex-1 text-end">
        <a @click="scrollToSkillsReference" class="block md:inline-block md:mr-4 pr-8">skills ↘︎</a>
        <a @click="scrollToProjectReference" class="block md:inline-block md:mr-4 pr-8">projects ↘︎</a>
        <a @click="scrollToAboutReference" class="block md:inline-block">about ↘︎</a>
      </div>
    </header>
    <Home/>
    <Skills ref="skills"/>
    <Projects ref="projects"/>
    <About ref="about"/>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
