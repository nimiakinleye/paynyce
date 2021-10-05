<template>
  <div
    class="
      p-6
      bg-yellow-400
      my-6
      rounded-lg
      text-white text-center
      md:text-left
    "
  >
    <div
      class="
        flex flex-col-reverse
        items-center
        md:flex-row
        justify-between
        md:items-end
      "
    >
      <div class="max-w-sm">
        <img class="mx-auto md:mx-0" src="~/assets/logo_allwhite.svg" alt="" />
        <h1 class="my-2 md:my-8 text-3xl font-bold">FlipTwice Music</h1>
        <p class="my-2 mb-4 md:my-8">
          Get that spice to your music with our music brand. Get good ears on
          your sound during and after the mix.
          <br />
          Record! Mix & Master
          <br />
          We do not
          play with the sound! But we play with the sound to get it on repeat a
          minimum of two times.
          <br />
          If you can't Flip it Twice it's not FlipTwice
        </p>
        <nuxt-link
          class="
            rounded-lg
            bg-white
            px-5
            py-2
            text-yellow-500
            hover:text-yellow-600
          "
          to="/"
          >Visit website</nuxt-link
        >
      </div>
      <div>
        <img
          class="md:w-64 mx-auto mb-4 md:mb-0 rounded-lg md:mx-0 md:ml-auto"
          src="~/assets/flipmusic.jpg"
          alt=""
        />
        <!-- <img
          class="md:w-96 mx-auto mb-4 md:mx-0 md:ml-auto md:-mb-6 pr-12"
          src="~/assets/flip_music.svg"
          alt=""
        /> -->
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
</style>