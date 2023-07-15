<script setup>
  defineProps({
    text: {
      type: String,
      required: true
    }
  })
</script>

<template>
  <p>{{ text }}</p>
</template>

<style scoped>
  p {
    color: #000;
    display: inline-flex;
    padding: 10px 20px 20px 20px;
    align-items: flex-start;
    gap: 10px;
  }  
</style>