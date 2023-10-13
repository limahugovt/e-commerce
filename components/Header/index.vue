<template>
    <div class="">
        <div class="h-9 bg-black text-white flex gap-3 items-center justify-center">
            <p>Sign up and get 20% off to your first order.</p>
            <a href="/" class="underline">Sign Up Now</a>
        </div>
        <div class="h-24 flex justify-center items-center">
            <div class="flex gap-10">
                <img src="@/assets/icons/Logo.svg" alt="Logo">

                <div class="flex gap-6 items-center">
                    <div class="flex">
                        <a href="">Shop</a>
                        <img src="@/assets/icons/ShopArrow.svg" alt="ShopArrow">
                    </div>
                    <a href="">On Sale</a>
                    <a href="">New Arrivals</a>
                    <a href="">Brands</a>
                </div>

                <div class="bg-BgSearch h-12 w-[577px] rounded-3xl flex py-3 px-4 gap-3">
                    <img src="@/assets/icons/SearchIcon.svg" alt="SearchIcon">
                    <input type="search" name="Search for products..." id="search" placeholder="Search for products..." class="w-full bg-BgSearch outline-0">
                </div>

                <div class="flex gap-4">
                    <img src="@/assets/icons/CartIcon.svg" alt="CartIcon">
                    <img src="@/assets/icons/UserConfig.svg" alt="">
                </div>
            </div>
        </div>
    </div>
</template>