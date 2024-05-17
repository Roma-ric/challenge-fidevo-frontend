<template>
  <nav>
    <!-- side bar content -->
    <aside class="sidebar fixed-left">
      <div class="side-inner px-3 py-3 ">
        <div class="d-flex justify-content-center align-items-center mb-4">
          <img src="../src/assets/walmart_favicon.png" alt="" width="30" height="30">
          <button class="btn btn-primary mx-3" style="border-radius: 15px;"> Sign in or create account </button>
        </div>
        <div class="d-flex">
          <img
            src="//i5.walmartimages.com/dfw/63fd9f59-ac39/29c6759d-7f14-49fa-bd3a-b870eb4fb8fb/v1/wplus-icon-blue.svg"
            alt="" width="20" height="20">
          <p class="mx-2 my-0"> Walmart+ </p>
        </div>
        <hr>
        <SideBarElement libelle="Purchase History" icon="receipt_long" />
        <SideBarElement libelle="My Items" icon="place_item" />
        <SideBarElement libelle="Account" icon="person" />
        <hr>
        <SideBarElement libelle="Help" icon="help" />
        <hr>
        <SideBarElement libelle="Lists" icon="favorite" />
        <SideBarElement libelle="Registries" icon="redeem" />
        <hr>
        <SideBarElement libelle="Departments" icon="grid_view" />
        <SideBarElement libelle="Services" icon="action_key" />
        <hr>
        <SideBarElement libelle="Give Feedback" icon="chat_bubble" />
      </div>
    </aside>

    <main>
      <header class="sticky-top" style="background-color: #0071DC;">

        <!-- header top -->
        <div class="px-2  py-4 row gx-2 align-items-center m-0 border-top-0 border-left-0 border-right-0 border-bottom">
          <div class="col d-lg-none d-md-flex d-none align-items-center">
            <a href="#" class="burger js-menu-toggle" data-toggle="collapse" data-target="#main-navbar">
              <span class=""></span>
            </a>
            <div class="header-element">
              <img src="../src/assets/walmart_favicon.png" alt="Walmart logo" style="width: 30px; margin-left: 10px;">
            </div>
          </div>
          <div class="col-3 d-lg-none d-md-none d-flex">
            <a href="#" class="burger js-menu-toggle" data-toggle="collapse" data-target="#main-navbar">
              <span class=""></span>
            </a>
            <img src="../src/assets/walmart_favicon.png" alt="Walmart logo" style="width: 30px; margin-left:5px;">
          </div>
          <div class="col d-lg-flex d-md-none d-none">
            <div class="header-element">
              <img src="../src/assets/walmartLogo.svg" alt="Walmart logo" style="width: 120px;">
            </div>
          </div>
          <div class="col d-lg-flex d-md-none d-none">
            <div class="header-element">
              <span class="material-symbols-outlined"> grid_view </span>
              <span class="fw-bold my-0 header-element-libelle"> Departments </span>
            </div>
          </div>
          <div class="col d-lg-flex d-md-none d-none">
            <div class="header-element">
              <span class="material-symbols-outlined"> action_key </span>
              <span class="fw-bold my-0 header-element-libelle"> Services </span>
            </div>
          </div>
          <div class="col-lg-5 col-md-9 col-7">
            <div class="card d-flex flex-row justify-content-center align-items-center rounded rounded-pill"
              style="height: 40px;">
              <input type="text" placeholder="Search everything at Walmart online and in store" id="search-input"
                class="form-control border-0 rounded rounded-pill d-lg-flex d-md-none d-none">
              <input type="text" placeholder="Search Walmart" id="search-input"
                class="form-control border-0 rounded rounded-pill d-lg-none d-md-flex d-flex">
              <span class="material-symbols-outlined p-1 m-1 rounded rounded-pill" style="background-color: #FFC220;">
                search </span>
            </div>
          </div>
          <div class="col d-lg-flex d-md-none d-none">
            <div class="header-element">
              <span class="material-symbols-outlined"> favorite </span>
              <div class="d-flex flex-column justify-content-start align-items-start">
                <p class="my-0 header-element-libelle" style="font-size: 13px;"> Reorder </p>
                <span class="fw-bold my-0 header-element-libelle"> My Items </span>
              </div>
            </div>
          </div>
          <div class="col d-lg-flex d-md-none d-none">
            <div class="header-element">
              <span class="material-symbols-outlined"> person </span>
              <div class="d-flex flex-column justify-content-start align-items-start">
                <p class="my-0 mx-2 header-element-libelle" style="font-size: 13px;"> Sign in </p>
                <span class="fw-bold my-0 header-element-libelle"> Account </span>
              </div>
            </div>
          </div>
          <div class="col-lg-1 col-md-1 col-2">
            <div class="header-element d-flex flex-column">
              <span class="material-symbols-outlined"> shopping_cart
                <span class=" position-absolute top-10 start-10 translate-middle badge rounded-pill bg-warning"
                  style="font-size: 10px;">
                  0
                  <span class="visually-hidden">unread messages</span>
                </span>
              </span>
              <p class="my-0 header-element-libelle" style="font-size: 13px;"> $0.00 </p>
            </div>
          </div>
        </div>

        <!-- header bottom -->
        <div class="d-flex justify-content-between align-items-center py-1">

          <!-- dropdown -->
          <div class="dropdown">
            <!-- button -->
            <button class="card border-0 d-flex justify-content-center flex-row dropdown-toggle text-light fw-bold px-4"
              type="button" id="dropdownMenuButton1" data-bs-toggle="dropdown" aria-expanded="false"
              style="background-color: #0071DC; font-size: 14px;">
              <img src="https://i5.walmartimages.com/dfw/4ff9c6c9-ad46/k2-_0a671c38-d307-447c-835e-7904ab143c26.v1.png"
                alt="" width="25" height="25">
              <span class="mx-2"> How do you want your items? </span>
              <div class="d-lg-flex d-md-flex d-none justidy-content-center align-items-center"
                style="font-size: 12px; font-weight: 15;">
                |
                <img
                  src="https://i5.walmartimages.com/dfw/4ff9c6c9-40c5/k2-_f5224bb5-3493-47da-a046-7f816ac1730e.v1.png"
                  alt="" width="20" height="20">
                <p class="mx-2 my-0"> Sacramento, 95829 </p>
                <img
                  src="https://i5.walmartimages.com/dfw/4ff9c6c9-cc5a/k2-_cb966ffb-2cf6-4a8d-869c-27d99919cb16.v1.png"
                  alt="" width="20" height="20">
                <p class="mx-2 my-0"> Sacramento Supercenter </p>
              </div>
            </button>
            <!-- content -->
            <div class="dropdown-menu col-lg-7 col-md-7 col-12 border-0 m-0 px-3"
              style="background-color: #0071DC; border-radius: 0px 0px 20px 20px" aria-labelledby="dropdownMenuButton1">
              <div class="d-flex justify-content-center mb-2">
                <div class="d-flex flex-column justify-content-center">
                  <img
                    src="https://i5.walmartimages.com/dfw/4ff9c6c9-486e/k2-_4be6f532-b0b2-4480-bb65-d53586e87193.v1.png"
                    alt="" width="50" height="50">
                  <span class="fw-bold text-light" style="font-size: 14px;"> Shipping </span>
                </div>
                <div class="d-flex flex-column justify-content-center mx-4">
                  <img
                    src="https://i5.walmartimages.com/dfw/4ff9c6c9-944a/k2-_333618e2-7327-4081-990e-7870dd062248.v1.png"
                    alt="" width="50" height="50">
                  <span class="fw-bold text-light" style="font-size: 14px;"> Pickup </span>
                </div>
                <div class="d-flex flex-column justify-content-center">
                  <img
                    src="https://i5.walmartimages.com/dfw/4ff9c6c9-4637/k2-_c8d39665-dac4-474a-9fb7-ab5feeb647b5.v1.png"
                    alt="" width="50" height="50">
                  <span class="fw-bold text-light" style="font-size: 14px;"> Delivery </span>
                </div>
              </div>
              <div class="card p-2 mb-2" style="border-radius: 7px;">
                <div class="d-flex flex-row">
                  <img
                    src="https://i5.walmartimages.com/dfw/4ff9c6c9-5249/k2-_71d3c250-050a-40b0-8fd7-c84c1df83204.v1.png"
                    alt="" width="20" height="20">
                  <div class="d-flex flex-column mx-2" style="font-size: 13px;">
                    <span class="fw-bold"> Add an address for shipping and delivery </span>
                    <p> Sacramento, CA 95829 </p>
                  </div>
                </div>
                <button class="btn btn-primary" style="background-color: #0071DC; border-radius: 13px;"> Add address
                </button>
              </div>
              <div class="card d-flex flex-row p-2 mb-3" style="border-radius: 7px;">
                <img
                  src="https://i5.walmartimages.com/dfw/4ff9c6c9-14f0/k2-_8ce34043-6050-4f39-afb2-3e76a554f8a3.v1.png"
                  alt="" width="20" height="20">
                <div class="d-flex flex-column mx-2" style="font-size: 13px;">
                  <span class="fw-bold"> Sacramento Supercenter </span>
                  <p> 8915 GERBER ROAD, Sacramento, CA 95829 </p>
                </div>
              </div>
            </div>
          </div>

          <!-- over link -->
          <div class="d-lg-flex d-md-flex flex-wrap d-none mx-4">
            <router-link to="/"> Deals </router-link>
            <div class="d-lg-flex d-md-none d-none">
              <router-link to="/"> Mother's Day </router-link>
            <router-link to="/"> Grocery & Essentials </router-link>
              <router-link to="/"> Teacher Apprecitaion </router-link>
              <router-link to="/"> Home </router-link>
              <router-link to="/"> Fashion </router-link>
              <router-link to="/"> Electronics </router-link>
            </div>
          </div>

        </div>

      </header>
      <div class="position-relative">
        <router-view />
      </div>
    </main>

  </nav>
</template>

<script setup lang="ts">
import SideBarElement from './components/SideBarElement.vue';

</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.header-element {
  color: white;
  padding: 10px;
  height: 45px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 14px;
}

.header-element:hover {
  background-color: #004F9A;
  border-radius: 25px;
}

.header-element-libelle {
  margin-left: 4px;
}

#search-input:focus {
  border: 0px solid white;
}

nav {
  a {
    font-weight: bold;
    color: #ffffff;
    text-decoration: none;
    margin-left: 15px;
    font-size: 14px;

    &.router-link-exact-active {
      color: #ffffff;
    }
  }

  a:hover {
    text-decoration: underline;
  }
}
</style>
