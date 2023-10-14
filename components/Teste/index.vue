<template>
  <div>
    <div class="top-bar bg-black text-white flex items-center justify-center h-9 gap-3 min-[320px]:text-xs md:text-base">
      <p class="">Sign up and get 20% off your first order.</p>
      <a href="/" class="underline">Sign Up Now</a>
    </div>

    <div class="nav-bar flex items-center justify-between lg:px-[100px] lg:py-6 min-[320px]:px-4 min-[320px]:py-5 gap-10">
      <div class="flex items-center gap-4">
        <img src="@/assets/icons/List.svg" alt="" class="flex min-[1450px]:hidden" @click="toggleSidebar">
        <img src="@/assets/icons/Logo.svg" alt="Logo">
      </div>

      <div class="menu gap-6 items-center min-[320px]:hidden min-[1450px]:flex">
        <div class="flex">
            <a href="">Shop</a>
            <img src="@/assets/icons/ShopArrow.svg" alt="">
        </div>
        <a href="">On Sale</a>
        <a href="">New Arrivals</a>
        <a href="">Brands</a>
      </div>

      <div class="search-bar bg-BgSearch rounded-3xl lg:w-[36rem] md:w-96 hidden md:flex min-w-[320px] p-3 gap-3">
        <img src="@/assets/icons/SearchIcon.svg" alt="SearchIcon">
        <input type="search" name="Search for products..." id="search" placeholder="Search for products..." class="w-full bg-BgSearch outline-0">
      </div>

      <div class="icons flex gap-4">
        <img src="@/assets/icons/SearchIcon.svg" alt="CartIcon" class="flex md:hidden">
        <img src="@/assets/icons/CartIcon.svg" alt="CartIcon">
        <img src="@/assets/icons/UserConfig.svg" alt="" @click="toggleSidebar">
      </div>
    </div>
  </div>
  <div class="h-full w-40 bg-black flex p-6 min-[1450px]:hidden absolute" :class="{'hidden': !isOpen}">
    <div class="grid text-white h-4 gap-3">
        <a href="">- Shop</a>
        <a href="">- On Sale</a>
        <a href="">- New Arrivals</a>
        <a href="">- Brands</a>
      </div>
  </div>
</template>

<script>
    export default {
        data() {
            return {
                isOpen: false,
        };
      },
      methods: {
          toggleSidebar() {
              this.isOpen = !this.isOpen;
        }
      }
    };
  </script>
