<template>
    
    <div class="z-50 flex flex-col justify-center items-center">
        <div class="mt-20">
            <h1 class="text-[#031d44] text-7xl font-semibold">About</h1>
            <hr class="mt-10 border-4 border-[#F87666] mx-[10%] w-[70%]">
        </div>
        <div class="py-10 md:px-16 w-full flex flex-col md:flex-row justify-center items-center mt-4">
            <div class="about-card">
                <h2 class="text-lg font-semibold text-center text-[#031d44]">What is Hackathon ?</h2>
                <p class="mt-2 text-[rgba(3,33,78,0.7)]">A hackathon is an invention and innovation competition for
                    technology. A hackathon is a
                    learning experience where students can come to use technology to learn new software, hardware,
                    skills,
                    and techniques by creating a project with a team of up to 4 people throughout the event.</p>
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
    <h2 class="index-module_type__E-SaG font-bold text-[20px] md:text-[48px] text-center text-[#00FFA3] mt-20"
        v-motion-slide-visible-bottom>This
        is Magnathon's Second Edition</h2>
    <h2 class="index-module_type__E-SaG text-[15px] md:text-[20px] text-center text-[#00FFA3] my-4"
        v-motion-slide-visible-bottom>Memories from
        1.0
    </h2>
    <hr class="border border-[#166F7B] mx-[10%] w-[80%]">
    <div class="carousel-container mt-6">
        <div class="carousel-track h-[350px] sm:h-[300px] lg:h-[200px]">
            <img src="../assets/images/img1.webp" class="carousel-img" alt="image 3 - magnathon '22">
            <img src="../assets/images/img4.webp" class="carousel-img" alt="image 4 - magnathon '22">
            <img src="../assets/images/img5.webp" class="carousel-img" alt="image 5 - magnathon '22">
            <img src="../assets/images/img6.webp" class="carousel-img" alt="image 6 - magnathon '22">
            <img src="../assets/images/img7.webp" class="carousel-img" alt="image 7 - magnathon '22">
            <img src="../assets/images/img8.webp" class="carousel-img" alt="image 8 - magnathon '22">
            <img src="../assets/images/img3.webp" class="carousel-img" alt="image 9 - magnathon '22">
        </div>
    </div>
</template>

<style scoped>
.about-card {
    width: 320px;
    height: 400px;
    background-color: #fffff2;
    padding: 1rem;
    border-radius: 0.75rem;
    margin: 1rem;
    border: #14374B 0.01rem solid;
    box-shadow: 0 .5rem 1rem rgba(0, 0, 0, .15) !important;
}

.about-carousel {
    box-shadow: 6px 6px #166F7B;
    width: 100%;
    border-radius: 1rem;
    border-width: 1px;
    --tw-border-opacity: 1;
    border-color: #166F7B;
}

span {
    border-right: .05em solid;
    animation: caret 1s steps(1) infinite;
}

.carousel-container {
    box-shadow: 0 8px #166F7B;
    position: relative;
    width: 100%;
    overflow: hidden;
    white-space: nowrap;
    border-bottom-width: 1px;
    border-color: #166F7B;
    --tw-bg-opacity: 1;
    background-color: #14374B;
}

.carousel-container:before {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 1;
    height: 100%;
    width: 100px;
    background-image: linear-gradient(to right, var(--tw-gradient-stops));
    --tw-gradient-from: var(--secondary-color) var(--tw-gradient-from-position);
    --tw-gradient-to: rgb(255 255 255 / 0) var(--tw-gradient-to-position);
    --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
    --tw-gradient-to: transparent var(--tw-gradient-to-position);
    content: ""
}

.carousel-container:after {
    position: absolute;
    top: 0;
    right: 0;
    z-index: 1;
    height: 100%;
    width: 100px;
    background-image: linear-gradient(to right, var(--tw-gradient-stops));
    --tw-gradient-from: transparent var(--tw-gradient-from-position);
    --tw-gradient-to: rgb(0 0 0 / 0) var(--tw-gradient-to-position);
    --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
    --tw-gradient-to: var(--secondary-color) var(--tw-gradient-to-position);
    content: ""
}

.carousel-track {
    animation: 20s slide infinite linear;
    display: flex;
    width: 100%;
    padding-top: 2rem;
    padding-bottom: 2rem
}

@media (min-width: 768px) {
    .carousel-track {
        height: 500px;
        padding-top: 4rem;
        padding-bottom: 4rem
    }
}

.carousel-img {
    box-shadow: 4px 4px #166F7B;
    margin-left: 1.25rem;
    margin-right: 1.25rem;
    height: 100%;
    border-radius: .5rem;
    border-width: 1px;
    --tw-border-opacity: 1;
    border-color: #166F7B;
}

@keyframes slide {
    0% {
        transform: translate(0)
    }

    to {
        transform: translate(-130%)
    }
}

@media (max-width: 538px) {
    @keyframes slide {
        0% {
            transform: translate(0)
        }

        to {
            transform: translate(-500%)
        }
    }
}

@media (max-width: 768px) {
    @keyframes slide {
        0% {
            transform: translate(0)
        }

        to {
            transform: translate(-240%)
        }
    }
}

@media (max-width: 768px) {
    .carousel-container {
        box-shadow: 0 4px 0 0 var(--border-main-color)
    }

    .carousel-img {
        box-shadow: 2px 2px 0 0 var(--border-main-color)
    }
}
</style>

<script setup>


</script>