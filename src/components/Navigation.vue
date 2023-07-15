<template>
  <nav class="navbar sticky-top navbar-light">
    <div class="container-fluid justify-content-between">
      <!-- Left elements -->
      <ul class="navbar-nav flex-row main-menu">
        <li class="nav-item mx-2">
          <a class="nav-link active" href="#">women</a>
        </li>
        <li class="nav-item mx-2">
          <a class="nav-link" href="#">plus</a>
        </li>
        <li class="nav-item mx-2">
          <a class="nav-link" aria-current="page" href="#">men</a>
        </li>
        <li class="nav-item mx-2">
          <a class="nav-link" aria-current="page" href="#">accessories</a>
        </li>
      </ul>
      <!-- Left elements -->

      <!-- Center elements -->
      <div class="flex-row d-none d-md-flex">
        <img 
          alt="Logo" 
          src="@/assets/images/logo.svg" />
      </div>
      <!-- Center elements -->

      <!-- Right elements -->
      <ul class="navbar-nav flex-row">
        <!-- Icons -->
        <li class="nav-item mx-2">
          <a class="nav-link" href="#">
            <img 
              alt="User Icon" 
              src="@/assets/icons/bx_bx-user.svg" />
          </a>
        </li>
        <li class="nav-item mx-2">
          <a class="nav-link" href="#">
            <img 
              alt="Shopping Cart Icon" 
              src="@/assets/icons/bx_bx-shopping-bag.svg" />
          </a>
        </li>
        <li class="nav-item mx-2">
          <a class="nav-link" href="#">
            <img 
              alt="Heart Icon" 
              src="@/assets/icons/bx_bx-heart.svg" />
          </a>
        </li>
        <li class="nav-item mx-2">
          <a class="nav-link" href="#">
            <img 
              alt="Support Icon" 
              src="@/assets/icons/bx_bx-support.svg" />
          </a>
        </li>
        <li class="nav-item mx-2">
          <a class="nav-link" href="#">
            <img 
              alt="Search Icon" 
              src="@/assets/icons/bx_bx-search.svg" />
          </a>
        </li>

        <li class="nav-item mx-2 dropdown">
          <a
            class="nav-link dropdown-toggle"
            href="#"
            id="navbarDropdown"
            role="button"
            data-mdb-toggle="dropdown"
            aria-expanded="false">
            <img 
              alt="Search Icon" 
              src="@/assets/icons/usa_flag.png" />
            <label class="ml-1">usd $</label>
          </a>
        </li>
      </ul>
      <!-- Right elements -->
    </div>
  </nav>
</template>

<style scoped>
  .navbar {
    background: #fff;
    height: 70px;
  }

  .dropdown {
    border-radius: 35px;
    border: 1px solid #F2F2F2;
    width: 110px;
    text-align: center;
  }

  .dropdown-toggle::after {
    content: url('@/assets/icons/ant-design_down-outlined.svg');
    vertical-align: 0;
    border: none;
  }
  .dropdown label{
    color: #000;
    text-align: center;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    text-transform: uppercase;
  }

  .main-menu > li > a {
    color: #000;
    text-align: center;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    text-transform: uppercase;
  } 

  .main-menu > li > a.active {
    font-weight: 600;
  } 
</style>