<template>
  <div class="newsletter">
    <div class="container"> 
      <div class="row">
        <div class="col-xs-12 col-lg-8 newsletter-text">
          sign up for exclusive deals and updates
        </div>
        <div class="col-xs-12 col-lg-4 newsletter-form">
            <div class="input-group">
              <input 
                type="text" 
                placeholder="your email address">
              <button 
                class="search-btn" 
                type="button">
                <img src="@/assets/icons/ant-design_right-outlined.svg">
              </button>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .newsletter {
    background: #000; 
  }
  .newsletter-text {
    color: #FFF;
    font-size: 32px;
    font-style: normal;
    font-weight: 800;
    line-height: normal;
    text-transform: uppercase;
    padding: 18px 0px;
  }
  .newsletter-form input {
    background: #F2F2F2;
    color: #4D4D4D;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    text-transform: capitalize;
    border: 0!important;
    outline: 0!important;
    width: 88%;
    padding: 10px;
  }
  .search-btn {
    background: #fff!important;
    border: 0;
  }
  .newsletter-form .input-group {
    margin-top: 18px;
  }
</style>