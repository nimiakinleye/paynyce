<template>
  <div class="p-6 bg-blue-50 my-6 rounded-lg">
    <div class="flex flex-col-reverse md:flex-row justify-between">
      <div class="max-w-sm">
        <img class="w-32" src="~/assets/full_logo.svg" alt="" />
        <h1 class="my-2 md:my-8 text-3xl font-bold">FlipDidIt</h1>
        <p class="my-2 mb-4 md:my-8">
          Lights, Camera, Action! 
          <br />
          Video/Movie production at its best with a team
          dedicated to bring out the best from you and for you.
        </p>
        <nuxt-link class="rounded-lg bg-yellow-500 px-5 py-2 text-white hover:bg-yellow-600" to="/">Visit website</nuxt-link>
      </div>
      <div class="md:grid grid-cols-2 w-1/2 gap-6 hidden">
        <div class="flex flex-col justify-between">
          <img data-aos="zoom-in" class="rounded-lg" src="~/assets/did_it_1.png" alt="" />
          <img data-aos="zoom-in" class="rounded-lg" src="~/assets/did_it_2.png" alt="" />
        </div>
        <img data-aos="zoom-in"
          class="row-start-1 col-start-2 rounded-lg"
          src="~/assets/did_it_3.png"
          alt=""
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
</style>