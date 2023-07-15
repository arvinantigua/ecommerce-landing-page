<template>
  <div class="w-100 vip-exclusive"> 
    <div class="container">
      <div class="row">
        <div class="col">
          <div class="col-1 my-0">
            black friday exclusive
          </div>
        </div>
        <div class="col">
          <div class="col-2 col-2 mb-2 mt-3">
            free shipping on all orders for VIP 2 and up!
          </div>
        </div>
        <div class="col">
          <button type="button" class="p-2 mb-0 mt-3">
            shop now
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .vip-exclusive {
    background-image: url('@/assets/images/vip_exclusive_background.png'); 
    background-size: cover;
  }

  .vip-exclusive div.col-1 {
    color: #FFF;
    font-size: 32px;
    font-style: normal;
    font-weight: 800;
    text-transform: uppercase;
    width: 472px;
    line-height: 75px;
  }

  .vip-exclusive div.col-2 {
    color: #FFF;
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    text-transform: uppercase;
    width: 354px;
  }

  button {
    background: #FFF;
    color: #000;
    text-align: center;
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