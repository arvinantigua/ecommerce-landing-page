<script setup>
  import Heading from './Heading.vue'
  import { reactive } from 'vue'

  const data = reactive({ 
    recentlyBought: [
      {
        name: "Festive Looks Rust Red Ribbed Velvet Long Sleeve Bodysuit",
        image: "item-1.png",
        price: "$38",
        sale: "",
      },
      {
        name: "Chevron Flap Crossbody Bag",
        image: "item-2.png",
        price: "$5.77",
        sale: "$7.34",
      },
      {
        name: "Manilla Tan Multi Plaid Oversized Fringe Scarf",
        image: "item-3.png",
        price: "$29",
        sale: "$39",
      },
      {
        name: "Diamante Puff Sleeve Dress - Black",
        image: "item-4.png",
        price: "$45.99",
        sale: "",
      },
      {
        name: "Banneth Open Front Formal Dress in Black",
        image: "item-5.png",
        price: "$69",
        sale: "$99.95",
      },
    ]
  })
</script>

<template>
  <div class="container-fluid">
    <div class="row my-5">
      <div class="col text-center">
        <Heading label="Recently Bought" />
      </div>
    </div>
    <div class="row mt-3">
      <div class="w-100 col text-center">
        <div v-for="recent in data.recentlyBought" 
          class="recent-container mx-4 mb-4">
          <div>
            <img :src="`src/assets/images/${recent.image}`">
          </div>
          <div class="recent-name">
            {{ recent.name }}
          </div>
          <div class="recent-price">
            <span :class="[recent.sale ? 'on-sale' : '']">
              {{ recent.price }}
            </span>
            <span class="recent-price-sale">
              {{ recent.sale }}
            </span>
          </div>
        </div>
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
  .recent-name {
    color: #000;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    text-transform: capitalize;
    text-align: left!important;
    height: 50px;
  }
  .recent-price {
    color: #000;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    text-transform: capitalize;
    text-align: left!important;
  }
  .recent-price .on-sale {
    color: #c1272d;
  }
  .recent-price-sale {
    text-decoration-line: line-through;
    margin-left: 22px;
  }
</style>