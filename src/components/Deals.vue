<script setup>
  import Discount from './Discount.vue'
</script>

<template>
  <div class="container">
    <div class="row">
      <div class="col-xs-12 col-lg-2">
        <Discount 
          discount="$5" 
          text="on orders above $50" />
      </div>
      <div class="col-xs-12 col-lg-2">
        <Discount
          discount="$15" 
          text="on orders above $75" />
      </div>
      <div class="col-xs-12 col-lg-2">
        <Discount
          discount="$20" 
          text="on orders above $150" />
      </div>
      <div class="col-xs-12 col-lg-2">
        <Discount
          discount="$30" 
          text="on orders above $200" />
      </div>
      <div class="col-xs-12 col-lg-4 text-cecnter">
        <button type="button" class="my-5 p-2">
          check out all site-wide deals
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped>
  button {
    background: #000;
    color: #FFF;
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    text-transform: uppercase;
    margin-left: auto;
    margin-right: auto;
    display: block;
  }
</style>