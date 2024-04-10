<template>
    <div class="mt-20 timeline">
        <h1 class="text-[#031d44] text-7xl font-semibold">Timeline</h1>
        <hr class="mt-10 border-4 border-[#F87666] mx-[10%] w-[70%]">
    </div>
    <div class="flex flex-col justify-center items-center mt-8">
        <div class="flex flex-col justify-center items-center">
            <div class="time-box mt-4 w-[300px] rounded-2xl">
                <span class="font-bold">1st April 2024</span>
                <span>Registration Started</span>
            </div>
            <div class="time-box mt-4 w-[300px] rounded-2xl">
                <span class="font-bold">13th April 2024</span>
                <span>Registration Closed</span>
            </div>
            <div class="time-box mt-4 w-[300px] rounded-2xl">
                <span class="font-bold">15th April 2024</span>
                <span>Shortlisted Team Release</span>
            </div>
            <div class="grid grid-cols-2 gap-2">
                <button class="mt-4 w-[180px] lg:w-[300px] rounded-2xl"
                :class="[toggleId === 0 ? 'active' : 'time-box']"
                @click="toggleId = 0">
                    <span class="font-bold">17 April 2024</span>
                    <span>Day 1 Hacking</span>
                </button>
                <button class="time-box mt-4 w-[180px] lg:w-[300px] rounded-2xl"
                :class="[toggleId === 1 ? 'active' : 'time-box']"
                @click="toggleId = 1">
                    <span class="font-bold">18 April 2024</span>
                    <span>Day 2 Hacking</span>
                </button>
            </div>
        </div>
        <div class="w-full h-[650px] flex justify-center items-start mt-8 overflow-hidden">
            <div :class="[toggleId === 0 ? 'active-time' : 'inactive-time' ]">
                <div class="flex flex-col justify-between items-center">
                    <div class="mt-2 gap-4 flex">
                        <span>08 : 00 AM</span>
                        <span class="font-semibold">Offline Registration</span>
                    </div>
                    <hr class="mt-6 mb-10 border-2 border-[#F87666] mx-[10%] w-[70%]">
                </div>
                <div class="flex flex-col items-center justify-around">
                    <div class="mt-2 gap-4 flex">
                        <span>09 : 30 AM</span>
                        <span class="font-semibold">Inauguration</span>
                    </div>
                    <hr class="mt-6 mb-10 border-2 border-[#F87666] mx-[10%] w-[70%]">
                </div>
                <div class="flex flex-col items-center justify-around">
                    <div class="mt-2 gap-4 flex">
                        <span>10 : 30 AM</span>
                        <span class="font-semibold">Introduction Session</span>
                    </div>
                    <hr class="mt-6 mb-10 border-2 border-[#F87666] mx-[10%] w-[70%]">
                </div>
                <div class="flex flex-col items-center justify-around">
                    <div class="mt-2 gap-4 flex">
                        <span>12 : 30 PM</span>
                        <span class="font-semibold">Hack Begins</span>
                    </div>
                    <hr class="mt-6 mb-10 border-2 border-[#F87666] mx-[10%] w-[70%]">
                </div>
                <div class="flex flex-col items-center justify-around">
                    <div class="mt-2 gap-4 flex">
                        <span>08 : 00 PM</span>
                        <span class="font-semibold">Culturals</span>
                    </div>
                    <hr class="mt-6 mb-10 border-2 border-[#F87666] mx-[10%] w-[70%]">
                </div>
            </div>
            <div :class="[toggleId === 1 ? 'active-time' : 'inactive-time' ]">
                <div class="flex flex-col items-center justify-around">
                    <div class="mt-2 grid grid-cols-2 gap-4 justify-items-center justify-evenly">
                        <span>11 : 00 AM</span>
                        <span class="font-semibold">Hack Ends</span>
                    </div>
                    <hr class="mt-6 mb-10 border-2 border-[#F87666] mx-[10%] w-[70%]">
                </div>
                <div class="flex flex-col items-center justify-around">
                    <div class="mt-2 grid grid-cols-2 gap-4 justify-items-center justify-evenly">
                        <span>11 : 00 AM</span>
                        <span class="font-semibold">Project <br> Evaluation</span>
                    </div>
                    <hr class="mt-6 mb-10 border-2 border-[#F87666] mx-[10%] w-[70%]">
                </div>
                <div class="flex flex-col items-center justify-around">
                    <div class="mt-2 grid grid-cols-2 gap-4 justify-items-center justify-evenly">
                        <span>After <br> Evaluation</span>
                        <span class="font-semibold">Result <br> Announcement</span>
                    </div>
                    <hr class="mt-6 mb-10 border-2 border-[#F87666] mx-[10%] w-[70%]">
                </div>
                <div class="flex flex-col items-center justify-around">
                    <div class="mt-2 grid grid-cols-2 gap-4 justify-items-center justify-evenly">
                        <span>03 : 00 PM</span>
                        <span class="font-semibold">Project <br> Presentation</span>
                    </div>
                    <hr class="mt-6 mb-10 border-2 border-[#F87666] mx-[10%] w-[70%]">
                </div>
                <div class="flex flex-col items-center justify-around">
                    <div class="mt-2 grid grid-cols-2 gap-4 justify-items-center justify-evenly">
                        <span>Tech Fest <br> Inaugration</span>
                        <span class="font-semibold">Prize <br> Distribution</span>
                    </div>
                    <hr class="mt-6 mb-10 border-2 border-[#F87666] mx-[10%] w-[70%]">
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.time-box, .active{
    font-family: 'Orbitron';
    color: #fffff2;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 1.5rem;
}

.time-box{
    background: #031d44;
}

.timeline{
    display: flex;
    flex-direction: column;
    align-items: center;
}

.active{
    background: #e64b37;
}

.active-time{
    width: 100%;
    overflow: hidden;
}

.inactive-time{
    width: 0;
    overflow: hidden;
}

</style>

<script setup>
    import { ref } from 'vue';

    const toggleId = ref(0);

</script>