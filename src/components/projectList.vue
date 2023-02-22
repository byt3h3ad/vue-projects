<script>
import projects from "../assets/data.json";
export default {
  data() {
    return {
      projects: projects,
    };
  },
};
</script>

<template>
  <p v-for="item in projects" :key="item.id">
    <a href="{{ item.url }}">{{ item.name }}</a
    >: {{ item.description }}
  </p>
</template>
