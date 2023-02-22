<script setup>
const props = defineProps({
  time: {
    type: Number,
    required: true,
  },
});
const date = new Date(props.time * 1000);
</script>

<template>
  <hr />
  <p style="font-size: 0.8rem">last update: {{ date }}</p>
</template>
