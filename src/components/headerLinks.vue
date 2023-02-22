<script>
import links from "../assets/links.json";
export default {
  data() {
    return {
      links: links,
    };
  },
};
</script>

<template>
  <div align="right" v-for="item in links" :key="item.id">
    <a href="{{ item.uri }}">{{ item.name }}</a>
  </div>
</template>
