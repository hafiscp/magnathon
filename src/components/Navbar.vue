<template>
    <nav class="navbar glass">
        <div class="flex justify-center items-center">
            <button class="text-2xl md:hidden text-[#00FFA3] rounded-md ps-5" @click.prevent="toggle"><i
                    class="bi bi-list"></i></button>
        </div>
        <div id="mySidenav" class="sidenav" :class="{ 'activeNav': isNavActive }">
            <a href="javascript:void(0)" class="closebtn" @click="toggle">&times;</a>
            <a href="#homepage" @click="toggle">homepage</a>
            <a href="#about" @click="toggle">about</a>
            <a href="#timeline" @click="toggle">timeline</a>
            <a href="#faq" @click="toggle">FAQ</a>
        </div>
        <div class="optionsNavigation hidden md:flex">
            <a href="#homepage">
                <p class="hover:border-b-2 hover:border-[#F20605] hover:text-[#00FFA3] transition duration-500
                    ease-in-out transform hover:-translate-y-1 hover:scale-110"
                    :class="{ 'active': isActivePage == 'homepage' }">
                    homepage</p>
            </a>
            <a href="#about">
                <p class="hover:border-b-2 hover:border-[#F20605] hover:text-[#00FFA3] transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110"
                    :class="{ 'active': isActivePage == 'about' }">
                    about</p>
            </a>
            <a href="#timeline">
                <p class="hover:border-b-2 hover:border-[#F20605] hover:text-[#00FFA3] transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110"
                    :class="{ 'active': isActivePage == 'timeline' }">
                    timeline</p>
            </a>
            <a href="#faq">
                <p class="hover:border-b-2 hover:border-[#F20605] hover:text-[#00FFA3] transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110"
                    :class="{ 'active': isActivePage == 'faqs' }">
                    FAQ</p>
            </a>
        </div>
        <div class="logo ml-0 sm:ml-4">
            <img src="" alt="">
        </div>
    </nav>
</template>

<style scoped>
.navbar {
    position: fixed;
    top: 0;
    left: 0;
    height: 5rem;
    width: 100%;
    display: flex;
    justify-content: space-between;
    z-index: 1000;

}

.glass {
    background: transparent;
}

@media (min-width: 768px) {
    .glass{
        background: white;
            background: linear-gradient(to right bottom,
                    rgba(255, 255, 255, 0.4),
                    rgba(255, 255, 255, 0.2));
            backdrop-filter: blur(1rem);
    }
}

.optionsNavigation {
    color: #1DCC7E;
    width: 40%;
    justify-content: space-between;
    align-items: center;

}

.active {
    color: #00FFA3;
    border-bottom-width: 2px;
    border-bottom-color: #F20605;
    pointer-events: none;
}

.sidenav {
    height: 100%;
    width: 0;
    position: fixed;
    z-index: 1001;
    top: 0;
    left: 0;
    background-color: #166F7B;
    overflow-x: hidden;
    transition: 0.5s;
    padding-top: 60px;
}

.sidenav a {
    padding: 8px 8px 8px 32px;
    text-decoration: none;
    font-size: 25px;
    color: #1DCC7E;
    display: block;
    transition: 0.3s;
}

.sidenav a:hover {
    color: #00FFA3;
}

.sidenav .closebtn {
    position: absolute;
    top: 0;
    right: 25px;
    font-size: 36px;
    margin-left: 50px;
}

.activeNav {
    width: 250px;
}

@media screen and (max-height: 450px) {
    .sidenav {
        padding-top: 15px;
    }

    .sidenav a {
        font-size: 18px;
    }
}
</style>

<script setup>
import { ref } from 'vue';

let isNavActive = ref(false);
const isActivePage = ref('');
function toggle() {
    isNavActive.value = !isNavActive.value;
}

</script>