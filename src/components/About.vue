<template>

    <div class="z-50 flex flex-col justify-center items-center">
        <div class="mt-20">
            <h1 class="text-[#031d44] text-7xl font-semibold">About</h1>
            <hr class="mt-10 border-4 border-[#F87666] mx-[10%] w-[70%]">
        </div>
        <div class="py-10 md:px-16 w-full flex flex-col md:flex-row justify-center items-center mt-4">
            <div class="about-card">
                <h2 class="text-lg font-semibold text-center text-[#031d44]">What is Hackathon ?</h2>
                <p class="mt-2 text-[rgba(3,33,78,0.7)]">
                    
A hackathon is an invention and innovation competition focused on technology. It provides a learning experience where students can use technology to explore new software, hardware, skills, and techniques by creating a project with a team of up to 4 people over the event's duration. Hackathons encourage collaboration, creativity, and problem-solving, often tackling real-world challenges to develop innovative solutions.




</p>
            </div>
            <div class="about-card">
                <h2 class="text-lg font-semibold text-center text-[#031d44]">What is Magnathon ?</h2>
                <p class="mt-2 text-[rgba(3,33,78,0.7)]">Magnathon 2.0 is a 24-hour national-level hackathon hosted by
                    IEEE
                    Student Branch College of
                    Engineering Vadakara during the College's annual tech fest, Quasso Liberum 11. Our focus is on
                    tackling
                    sustainability challenges such as climate change, energy use, environmental monitoring, disaster
                    management, zero hunger, sustainable education, and tech-driven solutions aligned with the UN
                    Sustainable Development Goals for a better future.</p>
            </div>
        </div>
    </div>
    <div>
        <h3 class="text-2xl font-semibold text-center text-[#031d44]">Hack Starts In</h3>
    </div>
    <div class="flex justify-center items-center mt-2">
        <div class="time text-3xl">{{ days }}
            <div class="overlay flex flex-col justify-end items-center text-xl">
                Days
            </div>
        </div>
        <div class="hidden md:flex time-gap"> : </div>
        <div class="time text-3xl">{{ hours }}
            <div class="overlay flex flex-col justify-end items-center text-xl">
                Hrs
            </div>
        </div>
        <div class="hidden md:flex time-gap"> : </div>
        <div class="time text-3xl">{{ minutes }}
            <div class="overlay flex flex-col justify-end items-center text-xl">
                Mins
            </div>
        </div>
        <div class="hidden md:flex time-gap"> : </div>
        <div class="time text-3xl">{{ seconds }}
            <div class="overlay flex flex-col justify-end items-center text-xl">
                Sec
            </div>
        </div>
    </div>
</template>

<style scoped>
.about-card {
    width: 320px;
    height: 400px;
    text-align: center;
    background-color: #fffff2;
    padding: 1rem;
    border-radius: 0.75rem;
    margin: 1rem;
    border: #14374B 0.01rem solid;
    box-shadow: 0 .5rem 1rem rgba(0, 0, 0, .15) !important;
}

h3{
    font-family: 'Orbitron';
}

.time{
    width: 100px;
    height: 100px;
    background-color: #fffff2;
    padding: 1rem;
    border-radius: 0.75rem;
    margin: 0.2rem;
    border: #14374B 0.01rem solid;
    box-shadow: 0 .5rem 1rem rgba(0, 0, 0, .15) !important;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column; 
    font-family: 'Orbitron';
    position: relative;
}

.time-gap{
    width: 30px;
    height: 30px;
    background-color: #fffff2;
    padding: 1rem;
    border-radius: 0.75rem;
    margin: 1rem;
}

.overlay{
    width: 100%;
    height: 100%;
}

</style>

<script setup>
    import { ref, onMounted } from 'vue';

    const days = ref(0);
    const hours = ref(0);
    const minutes = ref(0);
    const seconds = ref(0);
    const countDownDate = new Date("Apr 17, 2024 09:00:00").getTime();

    const updateCountdown = () => {
        let now = new Date().getTime();
        let distance = countDownDate - now;

        days.value = Math.floor(distance / (1000 * 60 * 60 * 24));
        hours.value = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        minutes.value = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
        seconds.value = Math.floor((distance % (1000 * 60)) / 1000);
    };

    onMounted(() => {
        updateCountdown();
        setInterval(updateCountdown, 1000);
    });
</script>