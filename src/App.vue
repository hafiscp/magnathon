<script setup>
  import Navbar from './components/Navbar.vue'
  import Landing from './components/Landing.vue'
  import About from './components/About.vue'
  import Faqs from './components/Faqs.vue'
  import Sponsor from './components/Sponsor.vue'
  import Timeline from './components/Timeline.vue'
  import Tracks from './components/Tracks.vue'
  import PrizePool from './components/PrizePool.vue'
</script>

<template>
  <!-- <Navbar /> -->
  <section id="homepage" class="homepage flex flex-col md:flex-row justify-center items-center">
    <Landing />
  </section>
  <section id="about" class="flex min-h-screen flex-col items-center mt-2">
    <svg width="100%" height="100%" id="svg" viewBox="0 0 1440 690" xmlns="http://www.w3.org/2000/svg"
      class="transition duration-300 ease-in-out delay-150 absolute top-[-20vw] left-0 z-[-1]">
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
      <!-- <defs>
            <linearGradient id="gradient" x1="53%" y1="0%" x2="47%" y2="100%">
                <stop offset="5%" stop-color="#00d084"></stop>
                <stop offset="95%" stop-color="#8ED1FC"></stop>
            </linearGradient>
        </defs>
        <path
            d="M 0,700 L 0,408 C 112.07142857142858,455.375 224.14285714285717,502.75 350,495 C 475.85714285714283,487.25 615.5,424.37500000000006 733,409 C 850.5,393.62499999999994 945.8571428571429,425.75 1060,471 C 1174.142857142857,516.25 1307.0714285714284,574.625 1440,633 L 1440,700 L 0,700 Z"
            stroke="none" stroke-width="0" fill="url(#gradient)" fill-opacity="1"
            class="transition-all duration-300 ease-in-out delay-150 path-1" transform="rotate(-180 720 350)"></path> -->
    </svg>
    <About />
  </section>
  <section id="prize" class="flex min-h-screen flex-col items-center justify-center py-30">
    <PrizePool />
  </section>
  <section id="tracks" class="flex min-h-screen flex-col items-center justify-center py-30">
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
