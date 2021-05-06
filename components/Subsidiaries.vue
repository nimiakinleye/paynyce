<template>
  <div class="min-h-screen bg-sub-bg bg-cover py-32">
    <div class="my-container">
      <div class="flex flex-col lg:flex-row justify-between items-center">
        <div>
          <div class="flex justify-center items-center text-white mb-10">
            <div class="font-semibold uppercase">Our Subsidiaries</div>
            <div class="hidden md:inline my-line bg-white ml-4"></div>
          </div>
          <div class="flex flex-col items-center">
            <div class="h-36 w-72 my-bg my-bg-1 rounded-lg my-5 flex items-center justify-center">
              <div class="bg-overlay"></div>
              <div><img src="../static/flip.svg" alt=""></div>
            </div>
            <div class="h-36 w-72 my-bg my-bg-2 rounded-lg my-5 lg:ml-10 flex items-center justify-center">
              <div class="bg-overlay"></div>
              <div><img src="../static/flip.svg" alt=""></div>
            </div>
            <div class="h-36 w-72 my-bg my-bg-3 rounded-lg my-5 flex items-center justify-center">
              <div class="bg-overlay"></div>
              <div><img src="../static/flip.svg" alt=""></div>
            </div>
            <div class="h-36 w-72 my-bg my-bg-4 rounded-lg my-5 flex items-center justify-center">
              <div class="bg-overlay"></div>
              <div><img src="../static/flip.svg" alt=""></div>
            </div>
          </div>
        </div>
        <div class="lg:w-1/2 text-center lg:text-right text-white">
          <div class="text-5xl font-bold">
            <span class="my-color">Flippay</span><br />
          </div>
          <div class="my-10 max-w-xl mx-auto text-2xl lg:mx-0 lg:ml-auto">
            Sell your gift card and make money transfers to friends and family
          <br />
          <br />
            We offer gift card, money transfer via e-mail and bill payment services.
          <br />
          <br />
            We also offer Business solutions under the Flippay business platform.
          </div>
          <nuxt-link to="/" class="my-bg px-6 py-2 rounded">Visit Website</nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.my-bg-1 {
  background-image: url("../static/images/blue_phone.PNG");
}
.my-bg-2 {
  background-image: url("../static/images/vintage_phone.PNG");
}
.my-bg-3 {
  background-image: url("../static/images/man_working.PNG");
}
.my-bg-4 {
  background-image: url("../static/images/scenic_stage.PNG");
}

.my-bg {
  background-size: cover;
  position: relative;
}

.my-bg img {
  position: relative;
  z-index: 2;
}

.bg-overlay {
  height: 100%;
  width: 100%;
  background-color: black;
  opacity: 0.3;
  position: absolute;
  z-index: 1;
}
</style>