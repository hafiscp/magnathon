<script setup>
  import Navbar from './components/Navbar.vue'
  import Landing from './components/Landing.vue'
  import About from './components/About.vue'
  import Faqs from './components/Faqs.vue'
  import Sponsor from './components/Sponsor.vue'
  import Timeline from './components/Timeline.vue'
  import PrizePool from './components/PrizePool.vue'
</script>

<template>
  <Navbar />
  <section id="homepage" class="homepage flex flex-col md:flex-row justify-center items-center mt-20 sm:mx-10">
    <Landing />
  </section>
  <section id="about" class="flex min-h-screen flex-col items-center justify-center py-30">
    <About />
  </section>
  <!-- <section id="prize" class="flex min-h-screen flex-col items-center justify-center py-30">
    <PrizePool />
  </section> -->
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
</style>
