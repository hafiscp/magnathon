<template>
    <div class="mt-20 flex flex-col justify-center items-center">
        <h1 class="text-[#031d44] text-7xl font-semibold">FAQs</h1>
        <hr class="mt-10 border-4 border-[#F87666] mx-[10%] w-[70%]">
    </div>
    <div class="mt-4" v-for="(each, id) in faqs">
        <div class="w-[289px] sm:w-[550px] md:w-[750px] rounded-md border-10">
            <button class="flex w-full items-start justify-normal rounded-[5px] p-5 font-bold font-lg text-[#031d44]"
                @click="makeVisible(id)">
                <span class="me-2"><i class="bi bi-caret-down-fill"></i></span>
                <p class="text-start">{{ each.question }}</p>
            </button>
            <div class="overflow-hidden rounded-[5px] font-lg transition-[height] transition-1000 ease-in-out inActiveAnswer" ref="answer">
                <p class="ms-5 px-5 text-[#031d44]">
                    {{ each.answer }}
                </p>
            </div>
        </div>
    </div>
    <div class="flex flex-col items-center text-base h-full my-auto px-6 lg:px-0 mt-6">
        <div class="text-[#031d44]">Have More Questions</div>
        <h1 class="font-sans font-bold text-5xl text-center text-[#031d44]">Get in Touch</h1>
        <div class="font-sans text-center mt-8 w-full sm:w-4/5 lg:w-2/5 text-[#031d44]">
            Got questions, cool ideas, or just want to chat? We're all ears! Whether it's a tech glitch or you're unsure
            about team stuff, hit us up. Our virtual door is always open. Shoot us an email, drop a message, or slide
            into our DMs—we're here for you. Let's make this hackathon experience awesome together!
        </div>
        <div class="flex justify-around w-full sm:w-3/5 lg:w-1/5 mt-8 mb-8">
            <a href="https://www.instagram.com/magnathon" class="text-4xl text-[#F87666]">
                <i class="bi bi-instagram"></i>
            </a>
            <a href="https://www.linkedin.com/in/ieee-sb-cev-6aa3831b5" class="text-4xl text-[#F87666]">
                <i class="bi bi-linkedin"></i>
            </a>
            <a href="mailto:ieeesb@cev.ac.in" class="text-4xl text-[#F87666]">
                <i class="bi bi-envelope-at"></i>
            </a>
            <a href="https://wa.me/+919540216512" class="text-4xl text-[#F87666]">
                <i class="bi bi-whatsapp"></i>
            </a>
        </div>
    </div>

</template>

<script setup>
import { onMounted, ref } from 'vue'
const faqs = ref([
    {
        'question': 'How much is the participation fee?',
        'answer': "It's completely free!",
        opened: false,
        scrollheight: ''
    },
    {
        'question': 'Who all can participate?',
        'answer': `All undergraduate students from any college are welcome to participate. It is Free for all`,
        opened: false,
        scrollheight: ''
    },
    {
        'question': 'How many people per team?',
        'answer': "Two to four people per team.",
        opened: false,
        scrollheight: ''
    },
    {
        'question': 'What are the prerequisties needed?',
        'answer': "Hardware materials should bring by the participants. Other facilities to build will be provided.",
        opened: false,
        scrollheight: ''
    },
])

const answer = ref([])

function makeVisible(id) {
    if (answer.value[id].style.height == '') {
        answer.value[id].style.height = answer.value[id].scrollHeight + 'px';
    } else {
        answer.value[id].style.height = '';
    }
}

</script>

<style scoped>
h1{
    font-family: 'Orbitron';
}

.btn-opened {
    transform: rotate(45deg);
}


.inActiveAnswer {
    height: 0;
    overflow: hidden;
}
</style>
