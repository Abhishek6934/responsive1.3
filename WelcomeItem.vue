<template>
  <div class="WelcomeItem.vue">
    <h3>{{ projectTitle }}</h3>
    <p>{{ projectDescription }}</p>
  </div>
</template>

<script>
export default {
  props: ['projectTitle', 'projectDescription']
}
</script>

<style scoped>
.project-item {
  background-color: #fff;
  padding: 20px;
  margin: 10px;
  border-radius: 5px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
</style>


