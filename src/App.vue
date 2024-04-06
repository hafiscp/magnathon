<script setup>
  import Navbar from './components/Navbar.vue'
  import Landing from './components/Landing.vue'
  import About from './components/About.vue'
  import Faqs from './components/Faqs.vue'
  import Sponsor from './components/Sponsor.vue'
  import Timeline from './components/Timeline.vue'
  import Tracks from './components/Tracks.vue'
  import Why from './components/Why.vue'
</script>

<template>
  <Navbar />
  <section id="homepage" class="homepage flex flex-col md:flex-row justify-center items-center">
    <Landing />
  </section>
  <section id="about" class="">
    <svg width="1700px" height="100%" id="svg" viewBox="0 0 1440 690" xmlns="http://www.w3.org/2000/svg"
      class="transition duration-300 ease-in-out delay-150 absolute top-[-500px] md:top-[-340px] left-0 z-[-1] overflow-hidden">
      <defs>
        <linearGradient id="gradient" x1="53%" y1="0%" x2="47%" y2="100%">
          <stop offset="5%" stop-color="#00d084"></stop>
          <stop offset="95%" stop-color="#8ED1FC"></stop>
        </linearGradient>
      </defs>
      <path
        d="M 0,700 L 0,175 C 144.71428571428572,137.76785714285714 289.42857142857144,100.53571428571429 390,110 C 490.57142857142856,119.46428571428571 547,175.62499999999997 656,205 C 765,234.37500000000003 926.5714285714287,236.96428571428572 1066,265 C 1205.4285714285713,293.0357142857143 1322.7142857142858,346.5178571428571 1440,400 L 1440,700 L 0,700 Z"
        stroke="none" stroke-width="0" fill="url(#gradient)" fill-opacity="0.53"
        class="transition-all duration-300 ease-in-out delay-150 path-0" transform="rotate(-180 720 350)"></path>
    </svg>
    <div class="flex min-h-screen flex-col items-center mt-2">
      <About />
    </div>
  </section>
  <section class="flex min-h-screen flex-col items-center justify-center py-30 relative">
    <Why />
  </section>
  <section id="tracks" class="flex min-h-screen flex-col items-center justify-start py-30">
    <Tracks />
  </section>
  <section id="timeline" class="flex min-h-screen flex-col items-center justify-center py-30">
    <Timeline />
  </section>
  <section id="sponsors" class="flex min-h-screen flex-col items-center justify-center py-30">
    <Sponsor />
  </section>
  <section id="faq" class="min-h-screen flex flex-col items-center justify-center py-30 w-4/5 mx-auto">
    <Faqs />
  </section>
</template>

<style scoped>
  .homepage {
    height: calc(100vh - 5rem);
  }
  .image{
    background-image: url("./assets/images/img2.webp");
    background-position: center;
    background-size: cover;
  }
</style>
