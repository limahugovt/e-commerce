<template>
    <div class="w-[1240px] grid gap-[50px] m-auto">
        <div class="bg-black h-44 rounded-[20px] flex items-center px-16 py-9 justify-between">

            <div class="text-white font-bold text-[40px] max-w-[551px] leading-none	">
                <h1>STAY UPTO DATE ABOUT OUR LATEST OFFERS</h1>
            </div>

            <div class="flex flex-col gap-4">
                <div class="w-[350px] h-12 bg-white rounded-3xl flex py-3 px-4 gap-3">
                    <img src="@/assets/icons/MailIcon.svg" alt="Mail Icon">
                    <input type="email" name="email" id="email" placeholder="Enter your email address"
                        class="outline-none w-full">
                </div>
                <div class="w-[350px] h-12 bg-white rounded-3xl flex justify-center items-center py-3 px-4">
                    <button type="submit">Subscribe to Newsletter</button>
                </div>
            </div>
        </div>

        <div class="flex justify-between">

            <div class="w-[248px] h-[177px] grid gap-9">
                <img src="@/assets/icons/Logo.svg" alt="">
                <p>We have clothes that suits your style and which you’re proud to wear. From women to men.</p>
                <img src="@/assets/icons/Social.svg" alt="">
            </div>

            <div class="grid gap-7">
                <p class="font-semibold text-base">CONPANY</p>
                <ul class="grid gap-4">
                    <li>About</li>
                    <li>Features</li>
                    <li>Works</li>
                    <li>Carrer</li>
                </ul>
            </div>

            <div class="grid gap-7">
                <p class="font-semibold text-base">HELP</p>
                <ul class="grid gap-4">
                    <li>Customer Support</li>
                    <li>Delivery Details</li>
                    <li>Terms & Conditions</li>
                    <li>Privacy Policy</li>
                </ul>
            </div>
            
            <div class="grid gap-7">
                <p class="font-semibold text-base">FAQ</p>
                <ul class="grid gap-4">
                    <li>Acoount</li>
                    <li>Manege Delivery</li>
                    <li>Ordes</li>
                    <li>Payments</li>
                </ul>
            </div>

            <div class="grid gap-7">
                <p class="font-semibold text-base">RESOURCES</p>
                <ul class="grid gap-4">
                    <li>Free eBooks</li>
                    <li>Developmente Tutorialy</li>
                    <li>How to - Blog</li>
                    <li>Youtube  Playlist</li>
                </ul>
            </div>
        </div>

        <div class="mb-20">
            <hr class="border-solid border-b-[1px] border-gray-500">
            <p class="pt-6">Shop.co © 2000-2023, All Rights Reserved</p>
        </div>
    </div>
</template>