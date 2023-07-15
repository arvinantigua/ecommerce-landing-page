<script setup>
  defineProps({
    label: {
      type: String,
      required: true
    }
  })
</script>

<template>
  <label>{{ label }}</label>
</template>

<style scoped>
  label {
    color: #000;
    text-align: center;
    font-size: 36px;
    font-style: normal;
    font-weight: 800;
    line-height: normal;
    text-transform: capitalize;
  }
</style>