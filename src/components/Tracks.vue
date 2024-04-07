<template>
    <div class="mt-20 z-10 track-head">
        <h1 class="text-[#031d44] text-7xl font-semibold text-center">Tracks</h1>
        <hr class="mt-4 md:mt-10 border-4 border-[#F87666] mx-[10%] w-[70%]">
    </div>
    <div class="relative mt-16">
        <div class="flex justify-between items-center">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                <div class="tracks w-[270px] sm:w-[450px] md:w-[350px] h-[250px] sm:h-[180px] md:h-[560px] flex flex-col justify-start items-start p-2 rounded-xl overflow-y-scroll relative"
                    style="scrollbar-width: none;" v-for="track in tracks">
                    <div class="block">
                        <div class="flex justify-between">
                            <span class="text-black mt-2 mx-2 font-bold text-xl">{{ track.heading }}</span>
                            <img :src="track.imgSrc" alt="Goals" class="w-24 md:w-36 mt-2 ms-2 inline">
                        </div>
                        <p class="text-black mt-2 font-light">{{ track.subHeading }}</p>
                        <p class="text-black mt-2 hidden md:block">{{ track.ulHeading }}
                        <ul v-for="list in track.lists" class="list-disc list-inside">
                            <li>{{ list }}</li>
                        </ul>
                        </p>
                    </div>
                    <div class="md:hidden absolute bottom-4 right-4">
                        <button class="text-3xl text-black" @click="track.active = !track.active"><i
                                class="bi bi-arrow-up-short"></i></button>
                    </div>
                    <div class="w-full fixed z-50 bottom-[-18%] left-0 overflow-hidden duration-300"
                        :style="[track.active ? 'height: 100%' : 'height: 0%']">
                        <div class="text-[#031d44] w-full flex justify-end text-3xl">
                            <button @click="track.active = !track.active"><i class="bi bi-x me-8 mb-4"></i></button>
                        </div>
                        <div class="sm-tracks h-[80%] rounded-t-3xl">
                            <div class="block p-4 overflow-scroll">
                                <div class="flex justify-between">
                                    <img :src="track.imgSrc" alt="Goals" class="w-24 md:w-36 mt-2 ms-2 inline">
                                    <span class="text-[#fffff2] mt-2 mx-2 font-bold text-xl">{{ track.heading }}</span>
                                </div>
                                <p class="text-[white] mt-2 font-bold">{{ track.subHeading }}</p>
                                <p class="text-[white] mt-2">{{ track.ulHeading }}
                                <ul v-for="list in track.lists" class="list-disc list-inside">
                                    <li>{{ list }}</li>
                                </ul>
                                </p>
                            </div>
                        </div>

                    </div>
                </div>
                <!-- <div class="tracks w-[270px] sm:w-[450px] md:w-[350px] h-[250px] sm:h-[180px] md:h-[560px] flex flex-col justify-start items-start px-2 rounded-xl overflow-y-scroll"
                    style="scrollbar-width: none;">
                    <div>
                        <div class="flex justify-between">
                            <img src="/src/assets/images/disasterManagement.png" alt="Goals"
                                class="w-24 md:w-36 mt-2 ms-2 inline">
                            <span class="text-black mt-2 ms-2 font-bold text-md sm:text-xl">6. Disaster
                                Management</span>
                        </div>
                        <p class="text-black mt-2 font-bold">Enhance Resilience & Preparedness for Effective Disaster
                            Management</p>
                        <p class="text-black mt-2 hidden md:block">
                            Targets:
                        <ul class="text-white list-disc list-inside hidden md:block">
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
                    <div class="md:hidden absolute bottom-4 right-4">
                        <button class="text-3xl text-white" @click="disasterActive = !disasterActive"><i
                                class="bi bi-arrow-up-short"></i></button>
                    </div>
                    <div class="w-full fixed z-50 bottom-[-18%] left-0 overflow-hidden duration-300"
                        :style="[disasterActive ? 'height: 100%' : 'height: 0%']">
                        <div class="text-[#031d44] w-full flex justify-end text-3xl">
                            <button @click="disasterActive = !disasterActive"><i class="bi bi-x me-8 mb-4"></i></button>
                        </div>
                        <div class="h-[80%] sm-tracks rounded-t-3xl">
                            <div class="p-4">
                                <div class="flex justify-between">
                                    <img src="/src/assets/images/disasterManagement.png" alt="Goals"
                                        class="w-24 md:w-36 mt-2 ms-2 inline">
                                    <span class="text-[#fffff2] mt-2 ms-2 font-bold text-md sm:text-xl">6. Disaster
                                        Management</span>
                                </div>
                                <p class="text-[#fffff2] mt-2 font-bold">"Enhance Resilience and Preparedness for Effective
                                    Disaster
                                    Management"</p>
                                <p class="text-[#fffff2] mt-2">
                                    Targets:
                                <ul class="text-[#fffff2] list-disc list-inside">
                                    <li>Develop or enhance early warning systems using real-time data.</li>
                                    <li> Create platforms for efficient coordination among first responders,
                                        organizations,
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
                </div> -->
            </div>
        </div>
    </div>
</template>

<style scoped>
h1{
    font-family: 'Orbitron';
}

.active {
    border-bottom: 8px;
    border-top-left-radius: 15px;
    border-top-right-radius: 15px;
}

.tracks{
    background: linear-gradient(0deg,rgba(22, 111, 123, 0.9),rgba(22, 111, 123, 0.6), rgba(29,204,126,0.6));
    background: white;
    box-shadow: 0 .5rem 1rem rgba(0, 0, 0, .15) !important;
}

.track-head{
        display: flex;
        flex-direction: column;
        align-items: center;
}

.sm-tracks{
    background: linear-gradient(0deg,rgb(0, 0, 0),rgba(0, 43, 49, 0.9), rgba(0, 0, 0, 0.9));
}


</style>

<script setup>
import { ref } from 'vue';


const tracks = ref([
    {
        heading: `1. Zero Hunger`,
        subHeading: `End hunger, achieve food security, improve nutrition, and promote sustainable agriculture.`,
        ulHeading: `Targets:`,
        lists: [
            `A technology to reduce food scarcity.`,
            `A system for distributing nutritious food.`,
            `A mechanism to manage wastage of food.`
        ],
        imgSrc: '/src/assets/images/goal2.png',
        active: false
    },
    {
        heading: `2. Climate Change`,
        subHeading: `Take urgent action to combat climate change and its impacts.`,
        ulHeading: `Targets:`,
        lists: [
            `Integrate climate change measures into national policies, strategies, and planning.`,
            `Improve education, awareness-raising, and human and institutional capacity on climate change mitigation, adaptation, impact reduction, and early warning.`,
            `Strengthen resilience and adaptive capacity to climate-related hazards and natural disasters worldwide.`,
            `Promote mechanisms for raising capacity for effective climate change-related planning and management.`
        ],
        imgSrc: '/src/assets/images/goal13.png',
        active: false
    },
    {
        heading: `3. Affordable and Clean Energy`,
        subHeading: `Ensure access to affordable, reliable, sustainable and clean energy for all.`,
        ulHeading: `Targets:`,
        lists: [
            `Ensure access to affordable, reliable, and modern energy services.`,
            `Substantially increase the share of renewable energy in the total energy mix.`,
            `Improve energy efficiency.`,
            `Expand infrastructure and upgrade technology for supplying modern and sustainable energy services.`
        ],
        imgSrc: '/src/assets/images/goal7.png',
        active: false
    },
    {
        heading: `4. Clean Water and Sanitation`,
        subHeading: `Ensure access to water and sanitation for all.`,
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
        active: false
    },
    {
        heading: `5. Responsible Consumption & Production`,
        subHeading: `Ensure sustainable consumption and production patterns.`,
        ulHeading: `Targets:`,
        lists: [
            `Implement cleaner production technologies for reduced environmental impact.`,
            `Embrace sustainable sourcing and fair trade practices.`,
            `Transition to a circular economy for waste reduction and resource optimization.`,
            `Strengthen waste management and disposal policies.`,
            `Educate and empower consumers to make sustainable choices.`
        ],
        imgSrc: '/src/assets/images/goal12.png',
        active: false
    },
    {
        heading: `6. Disaster Management`,
        subHeading: `Enhance Resilience & Preparedness for Effective Disaster Management`,
        ulHeading: `Targets:`,
        lists: [
            `Develop or enhance early warning systems using real-time data.`,
            `Create platforms for efficient coordination among first responders, organizations, and communities during disaster response.`,
            `Empower communities to build resilience through education, training, and planning.`,
            `Create innovative solutions for temporary shelters, emergency housing, and essential infrastructure in disaster-affected areas.`,
        ],
        imgSrc: '/src/assets/images/disasterManagement.png',
        active: false
    }
]);

const disasterActive = ref(false);

</script>