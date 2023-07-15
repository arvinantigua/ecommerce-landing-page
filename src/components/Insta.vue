<script setup>
  import Heading from './Heading.vue'
  import Paragraph from './Paragraph.vue'
  import { reactive } from 'vue'

  const data = reactive({ 
    inspos: [
      {
        image: "inspo-1.png",
      },
      {
        image: "inspo-2.png",
      },
      {
        image: "inspo-3.png",
      },
      {
        image: "inspo-4.png",
      },
      {
        image: "inspo-5.png",
      },
    ]
  })
</script>

<template>
  <div class="container-fluid">
    <div class="row mt-5">
      <div class="col text-center">
        <Heading label="your next inspo" />
      </div>
    </div>
    <div class="row mt-3">
      <div class="col text-center">
        <Paragraph text="Checkout who’s wearing what by using #THREADEDInspo on Instagram" />
      </div>
    </div>
    <div class="row mt-3">
      <div class="w-100 col text-center">
        <div v-for="inspo in data.inspos" 
          class="recent-container mx-4 mb-4">
          <div>
            <img :src="`src/assets/images/${inspo.image}`">
          </div>
        </div>
      </div>
    </div>
    <div class="row mt-3 mb-5">
      <div class="w-100 col text-center">
        <button 
          type="button" 
          class="py-2 px-3">
          view all posts
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .recent-container {
    display: inline-block;
    width: 225px; 
    vertical-align: top;
  }
  button {
    background: #000;
    color: #FFF;
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    text-transform: uppercase;
  }
</style>