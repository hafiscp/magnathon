<template>
    <hr class="border border-[#166F7B] mx-[10%] w-[80%]">
    <h1 class="index-module_type__E-SaG font-bold text-[20px] sm:text-[36px] md:text-[48px] text-center my-[3%] text-[#00FFA3]"
        id="header" v-motion-slide-visible-bottom>
    </h1>
    <hr class="border border-[#166F7B] mx-[10%] w-[70%]">
    <div class="py-10 md:px-16" id="about">
        <div class="w-full flex flex-col justify-center items-center px-8">
            <div class="flex flex-col xl:flex-row w-[100%]">
                <div class="about-card flex flex-col justify-center w-[100%] xl:w-[50%] me-4 mb-4 order-2 xl:order-1 p-2 md:p-4"
                    v-motion-slide-visible-left>
                    <p class="text-[20px] 2xl:text-[36px] font-bold text-[#00FFA3] mb-2">What is Magnathon ?</p>
                    <p class="text-white">Magnathon 2.0 is a 24-hour national-level hackathon hosted by IEEE Student
                        Branch College of Engineering Vadakara during the College's annual tech fest, Quasso Liberum 11.
                        Our
                        focus is on tackling sustainability challenges such as climate change, energy use, environmental
                        monitoring, disaster management, zero hunger, sustainable education, and tech-driven solutions
                        aligned with the UN Sustainable Development Goals for a better future.</p>
                </div>
                <div class="xl:w-1/2 flex flex-col justify-center items-center relative order-1 xl:order-2 mb-4"
                    v-motion-slide-visible-right>
                    <div class="w-full flex items-center rounded-lg">
                        <img src="../assets/images/img1.jpg" class="about-carousel" alt="image 1 - magnathon '22">
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="py-10 md:px-16">
        <div class="w-full flex flex-col justify-center items-center px-8">
            <div class="flex flex-col xl:flex-row w-[100%]">
                <div class="xl:w-1/2 flex flex-col justify-center items-center relative xl:me-4 mb-4"
                    v-motion-slide-visible-left>
                    <div class="w-full flex items-center rounded-lg">
                        <img src="../assets/images/img2.jpg" class="about-carousel" alt="image 2 - magnathon '22">
                    </div>
                </div>
                <div class="about-card flex flex-col justify-center w-[100%] xl:w-[50%] me-4 mb-4 p-2 md:p-4"
                    v-motion-slide-visible-right>
                    <p class="text-[20px] 2xl:text-[36px] font-bold text-[#00FFA3] mb-2">About Magnathon 1.0</p>
                    <p class="text-white">The first edition of Magnathon, organized by IEEE SB CEV as part of Quasso
                        Liberum 10, received international recognition last year by earning a bronze medal in the Darrel
                        Chong Student Activity Award presented by IEEE. The event saw a huge registration of over 500
                        individuals, out of which 100 were shortlisted by a distinguished panel based on their abstract
                        submissions. The final event had 30 teams participating.</p>
                </div>

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
            <img src="../assets/images/img1.jpg" class="carousel-img" alt="image 3 - magnathon '22">
            <img src="../assets/images/img4.jpg" class="carousel-img" alt="image 4 - magnathon '22">
            <img src="../assets/images/img5.jpg" class="carousel-img" alt="image 5 - magnathon '22">
            <img src="../assets/images/img6.jpg" class="carousel-img" alt="image 6 - magnathon '22">
            <img src="../assets/images/img7.jpg" class="carousel-img" alt="image 7 - magnathon '22">
            <img src="../assets/images/img8.jpg" class="carousel-img" alt="image 8 - magnathon '22">
            <img src="../assets/images/img3.jpg" class="carousel-img" alt="image 9 - magnathon '22">
        </div>
    </div>
</template>

<style scoped>
.about-card {

    box-shadow: 6px 6px #166F7B;
    border-radius: 1rem;
    border-width: 1px;
    --tw-border-opacity: 1;
    border-color: #166F7B;
    --tw-bg-opacity: 1;
    background-color: #14374B;
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

@media (max-width: 538px){
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

document.addEventListener('DOMContentLoaded', function (event) {
    // array with texts to type in typewriter
    const dataText = ["Code, Solve, Repeat", "Innovation Starts Here", "Crack the Code, Shape the Future", "Challenge Accepted"];

    // type one text in the typwriter
    // keeps calling itself until the text is finished
    function typeWriter(text, i, fnCallback) {
        // chekc if text isn't finished yet
        if (i < (text.length)) {
            // add next character to h1
            document.querySelector("h1").innerHTML = text.substring(0, i + 1) + '<span aria-hidden="true"></span>';

            // wait for a while and call this function again for next character
            setTimeout(function () {
                typeWriter(text, i + 1, fnCallback)
            }, 100);
        }
        // text finished, call callback if there is a callback function
        else if (typeof fnCallback == 'function') {
            // call callback after timeout
            setTimeout(fnCallback, 700);
        }
    }
    // start a typewriter animation for a text in the dataText array
    function StartTextAnimation(i) {
        if (typeof dataText[i] == 'undefined') {
            setTimeout(function () {
                StartTextAnimation(0);
            }, 20000);
        }
        // check if dataText[i] exists
        if (i < dataText[i].length) {
            // text exists! start typewriter animation
            typeWriter(dataText[i], 0, function () {
                // after callback (and whole text has been animated), start next text
                StartTextAnimation(i + 1);
            });
        }
    }
    // start the text animation
    StartTextAnimation(0);
});

</script>