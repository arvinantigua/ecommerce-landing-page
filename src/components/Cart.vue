<template>
  <div class="dropdown-menu shopping-cart-dropdown" aria-labelledby="shopping-cart">
    <div class="container-fluid">

      <div class="row my-2 item-row">
        <div class="col-xs-4 col-lg-4 text-center">
          <img src="@/assets/images/item-1.png" width="100">
        </div>
        <div class="col-xs-8 col-lg-8 cart-desc">
          Festive Looks Rust Red Ribbed Velvet Long Sleeve Bodysuit
          <div class="mt-2 cart-remove-item">
            <button class="w-100">Remove</button>
          </div>
        </div>
      </div>

      <div class="row my-2 item-row">
        <div class="col-xs-4 col-lg-4 text-center">
          <img src="@/assets/images/item-2.png" width="100">
        </div>
        <div class="col-xs-8 col-lg-8 cart-desc">
          Chevron Flap Crossbody Bag
          <div class="mt-2 cart-remove-item">
            <button class="w-100">Remove</button>
          </div>
        </div>
      </div>

      <div class="row my-2 mt-4">
        <div class="col-xs-12 col-lg-12">
          <div class="mt-2">
            <button class="w-100">Checkout</button>
          </div>
        </div>
      </div>

    </div>
  </div>
</template>

<style scoped>
  .shopping-cart-dropdown {
    position: absolute!important;
    right: 10px;
    width: 400px;
    left: auto!important;
  }
  .cart-desc {
    position: relative;
  }
  .cart-remove-item {
    position: absolute;
    bottom: 0;
    left: 10px;
    right: 10px;
  }
  button {
    background: #000;
    color: #FFF;
    text-align: center;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    text-transform: uppercase;
    padding: 10px 0;
  }
</style>