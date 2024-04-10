<template>
    <svg id="sw-js-blob-svg" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg" class="absolute opacity-50">
        <defs>
            <linearGradient id="sw-gradient" x1="0" x2="1" y1="1" y2="0">
                <stop id="stop1" stop-color="rgba(29, 204, 126, 0.6)" offset="0%"></stop>
                <stop id="stop2" stop-color="rgba(22, 111, 123, 0.7)" offset="100%"></stop>
            </linearGradient>
        </defs>
        <path fill="url(#sw-gradient)" d="M19.4,-33.4C22.8,-31.7,21.6,-21.7,24.9,-14.8C28.1,-7.8,35.9,-3.9,38.1,1.3C40.2,6.4,36.9,12.9,33.4,19.4C29.9,26,26.3,32.6,20.7,34.7C15.1,36.7,7.6,34.1,2.2,30.4C-3.2,26.6,-6.5,21.7,-11.4,19.3C-16.4,16.9,-23.1,17.1,-28.1,14.3C-33.1,11.5,-36.4,5.7,-35.1,0.8C-33.8,-4.2,-27.8,-8.4,-24.1,-13.5C-20.5,-18.6,-19,-24.5,-15.3,-26C-11.7,-27.5,-5.8,-24.7,1.1,-26.6C8,-28.4,16,-35,19.4,-33.4Z" width="100%" height="100%" transform="translate(50 50)" stroke-width="0" style="transition: all 0.3s ease 0s;" stroke="url(#sw-gradient)"></path>
    </svg>
    <div class="mt-20 z-10">
        <h1 class="text-[#031d44] text-7xl font-semibold text-center">Why Join Us ?</h1>
        <hr class="mt-4 md:mt-10 border-4 border-[#F87666] mx-[10%] w-[70%]">
    </div>
    <div class="flex flex-col lg:flex-row justify-evenly items-center mt-16 z-10 w-full">
        <div class="flex flex-col justify-center items-center mt-12 lg:mt-56 order-2 lg:order-1">
            <div class="text-[#031d44] text-6xl"><i class="bi bi-lightbulb"></i></div>
            <h4 class="text-[#031d44] text-4xl font-semi-bold text-center">Build Innovative <br> Solutions</h4>
        </div>
        <div class="flex flex-col justify-center items-center order-1 lg:order-2">
            <h3 class="text-[#031d44] text-9xl font-bold">50K</h3>
            <h4 class="text-[#031d44] text-5xl font-semi-bold">Prize Pool</h4>
        </div>
        <div class="flex flex-col justify-center items-center mt-12 lg:mt-56 order-3">
            <div class="text-[#031d44] text-6xl"><i class="bi bi-people-fill"></i></div>
            <h4 class="text-[#031d44] text-4xl font-semi-bold text-center">Collabration & <br> Networking</h4>
        </div>
    </div>
    <br>
    <div class="mt-12 lg:mt-6 z-10 flex flex-col justify-center items-center">
        <h4 class="text-[#031d44] text-4xl font-semi-bold text-center">Register Now For Free</h4>
        <div class="flex flex-row justify-center items-center mt-8 first-letter:font-sans ">
            <a href="https://magnathon2024.devfolio.co/"
                class="border border-[#F87666] bg-[#ff2929] flex flex-row justify-center items-center p-2 rounded-lg">
                <!-- <img src="../assets/images/Logo.png" class="w-10 me-1" alt="Defolio"> -->
                <span class="inline-flex items-center text-[#fffff2] text-lg justify-center mx-5">
                    Register Now
                    <img src="../assets/images/arrow.png" class="h-4 ml-3" alt="" style="max-height: 1em; filter: invert(100%);">
                </span>
                
            </a>
        </div>
    </div>
</template>

<style scoped>
    h1,h2,h3,h4, a span{
        font-family: 'Orbitron';
    }
</style>