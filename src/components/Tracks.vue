<template>
    <div class="mt-32 mb-4">
        <div class="font-sans text-[#00FFA3] text-6xl text-center" v-motion-slide-visible-bottom>
            Tracks
        </div>
        <div class="font-sans text-[#1DCC7E] text-xl mt-8" v-motion-slide-visible-bottom>
            UN Goals we have selected for this year
        </div>
    </div>
    <div class="relative">
        <div class="flex justify-between items-center">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                <div class="w-[150px] sm:w-[210px] md:w-[260px] h-[1800px] sm:h-[2300px] md:h-[290px] flex flex-col justify-center items-center"
                    v-for="track in tracks" :style="{ backgroundColor: track.bgColor }">
                    <img :src="track.imgSrc" alt="track.name" class="rounded-sm min-w-full">
                    <span class="text-white text-xl font-semibold"></span>
                </div>
            </div>
        </div>
    </div>
    <div class="mt-8">
        <div class="font-sans text-[#1DCC7E] text-xl text-center" v-motion-slide-visible-bottom>
            Special Tracks
        </div>
        <div class="flex justify-center items-center mt-4">
            <div class="w-[150px] sm:w-[210px] md:w-[260px] h-[1800px] sm:h-[2300px] md:h-[290px] flex flex-col justify-center items-center"
                :style="{ backgroundColor: spcTrack.bgColor }">
                <img :src="spcTrack.imgSrc" alt="spcTrack.name" class="rounded-sm min-w-full">
                <span class="text-white text-xl font-semibold"></span>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .glass {
        background: white;
        background: linear-gradient(to right bottom,
                rgba(255, 255, 255, 0.4),
                rgba(255, 255, 255, 0.2));
        backdrop-filter: blur(1rem);
    }
    .active{
        border-bottom: 8px;
        border-top-left-radius: 15px;
        border-top-right-radius: 15px;
    }
</style>

<script setup>
    import { ref } from 'vue'

    const active = ref(0)

    const tracks = ref([
        {
            name: 'Goal 2',
            imgSrc: '/assets/images/goal2.png',
            bgColor:'#D19F2A'
        },
        {
            name: 'Goal 6',
            imgSrc: '/assets/images/goal6.png',
            bgColor:'#00AED9'
        },
        {
            name: 'Goal 7',
            imgSrc: '/assets/images/goal7.png',
            bgColor: '#FDB714'
        },
        {
            name: 'Goal 12',
            imgSrc: '/assets/images/goal12.png',
            bgColor: '#CD8B2A'
        },
        {
            name: 'Goal 13',
            imgSrc: '/assets/images/goal13.png',
            bgColor: '#48773C'
        },
    ])

    const spcTrack = ref({
        name: 'Disaster Management',
        imgSrc: '/assets/images/disasterManagement.png',
        bgColor: '#F35E5D'
    })


</script>