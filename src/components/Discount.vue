<script setup>
  defineProps({
    discount: {
      type: String,
      required: true
    },
    text: {
      type: String,
      required: true
    }
  })
</script>

<template>
  <div class="container-fluid py-5">
    <div class="row text-center">
      <div class="col-xs-12 discount">
        <label class="discount-1">{{ discount }}</label>
        <label class="ml-1 discount-2">off</label>
      </div>
      <div class="col-xs-12 description">
        {{ text }}
      </div>
    </div>
  </div>
</template>

<style>
  .description {
    color: #000;
    font-size: 10px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    text-transform: uppercase;
  }

  .discount-1 {
    color: #000;
    font-size: 32px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    vertical-align: sub;
  }

  .discount-2 {
    color: #000;
    font-size: 18px;
    font-style: normal;
    font-weight: 800;
    line-height: normal;
    text-transform: uppercase;
    margin-left: 15px;
  }
</style>