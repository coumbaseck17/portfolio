<script setup>
  import MySkillComponent from './mySkillsComponent.vue';
  const components = {
    'my-skill': MySkillComponent
  };

  const props = defineProps(['title', 'description']);
</script>

<template>
  <div class="bg-rose-50 p-8">
    <h1 class="mb-4">skills</h1>
    <p class="mb-8 nunito">Here are skills that I have acquired during my university years, my internship, as well as through my personal experiences.</p>
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4 nunito">
      <!-- Databases -->
      <MySkillComponent title="Databases" description="I have always been interested in database management.I am well-versed in both SQL and NoSQL, and I have utilized tools such as MySQL, MongoDB, PostgreSQL, Neo4j, and DynamoDB."/>
      <!-- Data Analysis -->
      <MySkillComponent  class="col-span-2 sm:col-span-1 lg:col-span-2" title="Data Analysis" description="During my studies, I worked on projects involving data analysis. I find it truly satisfying to delve into data and extract meaningful insights, using platforms like Power BI, Jupyter Notebook, or Hadoop." />
      <!-- Project Management -->
      <MySkillComponent class="col-span-2 sm:col-span-1 lg:col-span-2" title="Project Management" description="I have been involved in project management, and I have used tools such as Jira and Trello to manage tasks and monitor progress." />
      <!-- Backend -->
      <MySkillComponent title="Backend" description="I have developed backend applications using Spring Boot and Node.js during my studies and apprenticeship." />
      <!-- Frontend -->
      <MySkillComponent  title="Frontend" description="I also enjoy coding websites; I have regularly used Angular and am currently expanding my skills by learning Vue.js." />
      <!-- Communication -->
      <MySkillComponent  class="col-span-2 sm:col-span-1 lg:col-span-2" title="Communication" description="I have a passion for learning different languages. As a native Italian speaker, I am fluent in French, having completed my university degrees in France. Additionally, I speak English very effectively, thanks to my work experiences and personal efforts." />
    </div>
  </div>
</template>


<style scoped>

</style>