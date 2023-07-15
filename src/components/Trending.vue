<script setup>
  import Heading from './Heading.vue'
  import Paragraph from './Paragraph.vue'
  import { reactive } from 'vue'

  const data = reactive({ 
    trendingData: [
      {
        name: "winter fashion",
        image: "winter_fashion.png",
      },
      {
        name: "boots",
        image: "boots.png",
      },
      {
        name: "night out",
        image: "night_out.png",
      },
      {
        name: "holidays",
        image: "holidays.png",
      },
      {
        name: "outerwear",
        image: "outerwear.png",
      },
      {
        name: "white dresses",
        image: "white_dresses.png",
      },
      {
        name: "sweaters",
        image: "sweaters.png",
      },
      {
        name: "party",
        image: "party.png",
      },
    ]
  })
</script>

<template>
  <div class="container">
    <div class="row mt-5">
      <div class="col text-center">
        <Heading label="Now Trending" />
      </div>
    </div>
    <div class="row mt-3">
      <div class="col text-center">
        <Paragraph text="See what everyone’s wearing right now" />
      </div>
    </div>
    <div class="row mt-3">
      <div 
        v-for="trending in data.trendingData"
        class="col-xs-12 col-md-6 col-lg-3">
        <div class="trending-container mb-4">
          <div>
            <img :src="`src/assets/images/${trending.image}`">
          </div>
          <div class="trending-name">
            {{ trending.name }}
          </div>
        </div>
      </div>
    </div>
    <div class="row mt-3 mb-5">
      <div class="w-100 col text-center">
        <div class="hashtag py-2 px-3 mx-3">#Thanksgiving</div>
        <div class="hashtag py-2 px-3 mx-3">#NewYears</div>
        <div class="hashtag py-2 px-3 mx-3">#Knitted</div>
        <div class="hashtag py-2 px-3 mx-3">#Pajamas</div>
        <div class="hashtag py-2 px-3 mx-3">#WFH</div>
        <div class="hashtag py-2 px-3 mx-3">#FallFashion</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .trending-container {
    display: block;
    margin-left: auto; 
    margin-right: auto;
    width: 225px; 
  }
  .trending-name {
    color: #000;
    text-align: center;
    font-size: 24px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    text-transform: uppercase;
  }
  .hashtag {
    display: inline-block;
    border-radius: 50px;
    border: 1px solid #000;
    background: #FFF;
    color: #000;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
  }
</style>