<template>
  <div>
    <h1>Welcome to My Portfolio</h1>
    <ProjectItem
      v-for="project in projects"
      :key="project.id"
      :projectTitle="project.title"
      :projectDescription="project.description"
    />
  </div>
</template>

<script>
import ProjectItem from './components/WelcomeItem.vue';

export default {
  components: {
    ProjectItem
  },
  data() {
    return {
      projects: [
        { id: 1, title: 'Project 1', description: 'Description for Project 1' },
        { id: 2, title: 'Project 2', description: 'Description for Project 2' }
        // Add more projects as needed
      ]
    };
  }
}
</script>
