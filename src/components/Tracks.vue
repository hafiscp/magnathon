<template>
    <div class="mt-32 mb-4">
        <div class="font-sans text-[#00FFA3] text-6xl text-center" v-motion-slide-visible-bottom>
            Tracks
        </div>
    </div>
    <div class="relative mt-2">
        <div class="flex justify-between items-center">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                <div class="w-[250px] sm:w-[450px] md:w-[350px] h-[560px] flex flex-col justify-start items-start px-2 rounded-xl overflow-y-scroll"
                    style="background-color:rgba(67, 72, 69,0.5); scrollbar-width: none;" v-for="track in tracks">
                    <img :src="track.imgSrc" alt="Goals" class="w-24 md:w-36 mt-2 ms-2 inline">
                    <span class="text-white mt-2">{{ track.heading }}</span>
                    <p class="text-white mt-2 font-bold">{{ track.subHeading }}</p>
                    <p class="text-white mt-2">{{ track.ulHeading }}
                    <ul v-for="list in track.lists" class="list-disc list-inside">
                        <li>{{ list }}</li>
                    </ul>
                    </p>
                </div>
                <div class="w-[250px] sm:w-[450px] md:w-[350px] h-[560px] flex flex-col justify-start items-start px-2 rounded-xl overflow-y-scroll"
                    style="background-color:rgba(67, 72, 69,0.5);scrollbar-width: none;">
                    <img src="/src/assets/images/disasterManagement.png" alt="Goals"
                        class="w-24 md:w-36 mt-2 ms-2 inline">
                    <span class="text-white mt-2">Problem statement 6: Disaster Management</span>
                    <p class="text-white mt-2 font-bold">"The frequency of disasters is increasing due to various
                        factors, including climate
                        change, urbanization, population growth, environmental degrada?on, and socio-economic
                        vulnerabilities."</p>
                    <p class="text-white mt-2">
                        Targets:
                    <ul class="text-white list-disc list-inside">
                        <li>Develop or enhance early warning systems using real-time data.</li>
                        <li> Create platforms for efficient coordination among first responders, organizations,
                            and communities during disaster response.</li>
                        <li>Empower communities to build resilience through education, training, and
                            planning.</li>
                        <li>Create innovative solutions for temporary shelters, emergency housing, and
                            essential infrastructure in disaster-affected areas.</li>
                    </ul>
                    </p>
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
    border-color: rgb(67, 72, 69);
}

.active {
    border-bottom: 8px;
    border-top-left-radius: 15px;
    border-top-right-radius: 15px;
}
</style>

<script setup>
import { ref } from 'vue';


const tracks = ref([
    {
        heading: `Problem statement 1: Zero Hunger`,
        subHeading: `"End hunger, achieve food security, improve nutrition, and promote sustainable agriculture."`,
        ulHeading: `Targets:`,
        lists: [
            `A technology to reduce food scarcity.`,
            `A system for distributing nutritious food.`,
            `A mechanism to manage wastage of food.`
        ],
        imgSrc: '/src/assets/images/goal2.png',
        bg: '#D19F2A'
    },
    {
        heading: `Problem statement 2: Climate Change`,
        subHeading: `"Take urgent action to combat climate change and its impacts."`,
        ulHeading: `Targets:`,
        lists: [
            `Integrate climate change measures into national policies, strategies, and planning.`,
            `Improve education, awareness-raising, and human and institutional capacity on climate change mitigation, adaptation, impact reduction, and early warning.`,
            `Strengthen resilience and adaptive capacity to climate-related hazards and natural disasters worldwide.`,
            `Promote mechanisms for raising capacity for effective climate change-related planning and management.`
        ],
        imgSrc: '/src/assets/images/goal13.png',
        bg: ''
    },
    {
        heading: `Problem statement 3: Affordable and Clean Energy`,
        subHeading: `"Ensure access to affordable, reliable, sustainable and clean energy for all."`,
        ulHeading: `Targets:`,
        lists: [
            `Ensure access to affordable, reliable, and modern energy services.`,
            `Substantially increase the share of renewable energy in the total energy mix.`,
            `Improve energy efficiency.`,
            `Expand infrastructure and upgrade technology for supplying modern and sustainable energy services.`
        ],
        imgSrc: '/src/assets/images/goal7.png',
        bg: ''
    },
    {
        heading: `Problem statement 4: Clean Water and Sanitation`,
        subHeading: `"Ensure access to water and sanitation for all."`,
        ulHeading: `Targets:`,
        lists: [
            `Ensure safe and affordable drinking water for all.`,
            `Enhance water quality, wastewater treatment, and safe reuse.`,
            `Improve water-use efficiency and secure freshwater supplies.`,
            `Implement integrated water resources management.`,
            `Safeguard and restore water-related ecosystems.`,
            `Expand water and sanitation support in remote areas.`
        ],
        imgSrc: '/src/assets/images/goal6.png',
        bg: ''
    },
    {
        heading: `Problem statement 5: Responsible Production and Consumption`,
        subHeading: `"Ensure sustainable consumption and production patterns."`,
        ulHeading: `Targets:`,
        lists: [
            `Implement cleaner production technologies for reduced environmental impact.`,
            `Embrace sustainable sourcing and fair trade practices.`,
            `Transition to a circular economy for waste reduction and resource optimization.`,
            `Strengthen waste management and disposal policies.`,
            `Educate and empower consumers to make sustainable choices.`
        ],
        imgSrc: '/src/assets/images/goal12.png',
        bg: ''
    }
]);


</script>