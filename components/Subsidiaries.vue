<template>
  <div class="my-container">
    <div data-aos="fade-right" class="py-16">
      <div class="font-bold text-sm uppercase mb-10">Our subsidiaries</div>
      <div class="text-4xl opacity-80 max-w-md font-semibold">
        We’re the design secret ingredient missing from your financial life
      </div>
    </div>
    <div class="flex flex-col lg:grid grid-cols-12 gap-x-6 my-6">
      <div data-aos="fade-down-right" class="col-start-1 col-end-8">
        <Flippay />
      </div>
      <div data-aos="fade-down-left" class="col-start-8 col-end-13 my-5 lg:my-0">
        <Flipnyce />
      </div>
    </div>
    <Flipmusic data-aos="zoom-in"/>
    <FlipDidIt />
  </div>
</template>

<script>
import Flippay from '~/components/Flippay.vue'
import Flipnyce from '~/components/Flipnyce.vue'
import Flipmusic from '~/components/Flipmusic.vue'
import FlipDidIt from '~/components/FlipDidIt.vue'
export default {
  components: {
    Flippay,
    Flipnyce,
    Flipmusic,
    FlipDidIt,
  },
}
</script>

<style>
</style>