<template>
    <div class="mt-20 mb-10">
        <div class="font-sans text-[#00FFA3] text-6xl" v-motion-slide-visible-bottom>
            Tracks
        </div>
    </div>
    <div class="relative">
        <div class="flex justify-between items-center">
            <div class="grid grid-cols-1 gap-4">
                <div class="w-[320px] sm:w-[450px] md:w-[550px] h-[120px] rounded-sm flex justify-between" v-for="track in tracks" :style="{ backgroundColor: track.bgColor }">
                    <img :src="track.imgSrc" alt="track.name" class="">
                </div>
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
            imgSrc: '/src/assets/images/goal2.png',
            bgColor:'#D19F2A'
        },
        {
            name: 'Goal 6',
            imgSrc: '/src/assets/images/goal6.png',
            bgColor:'#00AED9'
        },
        {
            name: 'Goal 7',
            imgSrc: '/src/assets/images/goal7.png',
            bgColor: '#FDB714'
        },
        {
            name: 'Goal 12',
            imgSrc: '/src/assets/images/goal12.png',
            bgColor: '#CD8B2A'
        },
        {
            name: 'Goal 13',
            imgSrc: '/src/assets/images/goal13.png',
            bgColor: '#48773C'
        },
    ])


</script>