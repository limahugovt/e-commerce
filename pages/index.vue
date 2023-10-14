<template>
    <Teste/>
    <section class="bg-[url('@/assets/icons/ImageBack.svg')] h-[41.438rem] flex items-center w-[92.188rem] m-auto bg-BgSection">
        <div class="ml-[100px]">
            <div class="max-w-[577px] grid gap-8">
                <h1 class="font-bold text-[77px] leading-none">FIND CLOTHES THAT MATCHES YOUR STYLE</h1>
                <p>Browse through our diverse range of meticulously crafted garments, designed to bring out your individuality and cater to your sense of style.</p>
                <div class="bg-black h-[52px] w-[210px] rounded-3xl text-white py-4 px-[54px] flex justify-center items-center">
                    <button class="">Shop Now</button>
                </div>
            </div>
            <div class="flex gap-8 items-center pt-12">
                <div class="">
                    <h2 class="font-bold text-[40px]">200+</h2>
                    <p>International Brands</p>
                </div>
                <div class="h-[74px] bg-black w-[1px]"></div>
                <div class="">
                    <h2 class="font-bold text-[40px]">2,000+</h2>
                    <p>High-Quality Products</p>
                </div>
                <div class="h-[74px] bg-black w-[1px]"></div>
                <div class="">
                    <h2 class="font-bold text-[40px]">30,000+</h2>
                    <p>Happy Customers</p>
                </div>
            </div>
        </div>
    </section>
    <section class="bg-black h-[122px] flex px-[100px] items-center gap-[106px] justify-center">
        <img src="@/assets/logos/VersaceLogo.svg" alt="">
        <img src="@/assets/logos/ZaraLogo.svg" alt="">
        <img src="@/assets/logos/GucciLogo.svg" alt="">
        <img src="@/assets/logos/PradaLogo.svg" alt="">
        <img src="@/assets/logos/CcLogo.svg" alt="">
    </section>
    <main class="grid">
        <section class="mt-20 grid justify-center">
            <h1 class="text-5xl font-bold text-center">NEW ARRIVALS</h1>
            <div class="flex gap-5 mt-16">
                <div v-for="product in NewArrivalsProducts" :key="product.id" class="grid gap-2">
                    <div class="w-[295px] h-[298px] bg-BgProduct rounded-[20px]">
                        <img :src="`/_nuxt/assets/products/${String(product.image)}.svg`" alt=""  class="rounded-[20px]">
                    </div>
                    <p class="font-bold text-base">{{ product.name }}</p>
                    <div class="flex gap-3">
                        <img src="@/assets/products/Avaliations.svg" alt="">
                        <p>{{ product.avaliation }}</p>
                    </div>
                    <p class="font-bold text-2xl">{{ product.price }}</p>
                </div>
            </div>
            <div class="w-[218px] h-[52px] grid justify-center items-center border-gray-500 border-solid border-[1px] rounded-3xl m-auto mt-8">
                <button class="w-full h-full">View All</button>
            </div>
        </section>

        <section class="mt-20 grid justify-center">
            <h1 class="text-5xl font-bold text-center">TOP SELLING</h1>
            <div class="flex gap-5 mt-16">
                <div v-for="product in NewArrivalsProducts" :key="product.id" class="grid gap-2">
                    <div class="w-[295px] h-[298px] bg-BgProduct rounded-[20px]">
                        <img :src="`/_nuxt/assets/products/${String(product.image)}.svg`" alt=""  class="rounded-[20px]">
                    </div>
                    <p class="font-bold text-base">{{ product.name }}</p>
                    <div class="flex gap-3">
                        <img src="@/assets/products/Avaliations.svg" alt="">
                        <p>{{ product.avaliation }}</p>
                    </div>
                    <p class="font-bold text-2xl">{{ product.price }}</p>
                </div>
            </div>
            <div class="w-[218px] h-[52px] grid justify-center items-center border-gray-500 border-solid border-[1px] rounded-3xl m-auto mt-8 mb-16">
                <button class="w-full h-full">View All</button>
            </div>
        </section>

        <section class="w-[1239px] h-[866px] bg-BgSearch rounded-[40px] m-auto">
            <div class="mt-[70px] mb-[70px]">
                <h1 class="text-5xl font-bold text-center">BROWSE BY DRESS STYLE</h1>
            </div>
            <div class="grid gap-5 justify-center">
                <div class="flex gap-5 h-[289px]">
                    <div class="w-[407px] h-[289px] rounded-[20px] bg-white">
                        <img src="@/assets/sections/CasualBg.svg" alt="" class="absolute rounded-[20px]">
                        <h1 class="font-bold text-4xl relative pl-9 pt-[25px]">Casual</h1>
                    </div>
    
                    <div class="w-[684px] h-[289px] rounded-[20px] bg-white">
                        <img src="@/assets/sections/Formal.svg" alt="" class="absolute rounded-[20px]">
                        <h1 class="font-bold text-4xl relative pl-9 pt-[25px]">Formal</h1>
                    </div>
                </div>
                
                <div class="flex gap-5 h-[289px]">
                    <div class="w-[684px] h-[289px] rounded-[20px] bg-white">
                        <img src="@/assets/sections/PatyBg.svg" alt="" class="absolute rounded-[20px]">
                        <h1 class="font-bold text-4xl relative pl-9 pt-[25px]">Paty</h1>
                    </div>
    
                    <div class="w-[407px] h-[289px] rounded-[20px] bg-white">
                        <img src="@/assets/sections/GymBg.svg" alt="" class="absolute rounded-[20px] pl-12">
                        <h1 class="font-bold text-4xl relative pl-9 pt-[25px]">Gym</h1>
                    </div>
                </div>
            </div>
        </section>
    </main>
    <Footer class="mt-20"/>
</template>
<script setup>
const NewArrivalsProducts = [
    {
        id: '1',
        image: 'Tshirt',
        name: 'T-SHIRT WITH TAPE DETAILS',
        avaliation: '4.5',
        price: '$120'
    },
    {
        id: '2',
        image: 'Tshirt',
        name: 'SKINNY FIT JEANS',
        avaliation: '3.5',
        price: '$240'
    },
    {
        id: '3',
        image: 'Tshirt',
        name: 'CHECKERED SHIRT',
        avaliation: '4.5',
        price: '$180'
    },
    {
        id: '4',
        image: 'Tshirt',
        name: 'SLEEVE STRIPED T-SHIRT',
        avaliation: '4.5',
        price: '$130'
    }
]

</script>