<template>
  <div class="my-container">
    <div
      class="flex flex-col-reverse lg:grid grid-cols-2 gap-x-12 py-12 lg:py-32 items-center"
    >
      <div class="max-w-lg text-center lg:text-left">
        <div class="font-bold text-sm uppercase mt-10 lg:mt-0">About us</div>
        <div class="font-semibold my-5">
          This company is all about what’s new, quality and functionality.
        </div>
        <div class="text-gray-600 my-5">
          We started this journey in 2020 and have since then grown our brand up. We have a team dedicated to building the brand and its trade partners. All businesses registered under this company are independent of operations enabling effective work flow.
        </div>
        <div class="flex uppercase justify-center lg:justify-start items-center">
          <div class="hidden md:inline my-line bg-black"></div>
          <nuxt-link to="/" class="mx-4 font-semibold"
            >Know more about us</nuxt-link
          >
          <div>
            <svg
              class="w-4"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 -66 511.9995 511"
            >
              <path
                d="m326.390625 380.460938c-6.507813 0-13.085937-1.265626-19.375-3.871094-18.832031-7.792969-31-25.929688-31-46.203125v-43.03125c0-11.046875 8.953125-20.003907 20-20.003907s20.003906 8.957032 20.003906 20.003907v43.03125c0 5.992187 4.402344 8.457031 6.292969 9.242187 1.925781.796875 6.871094 2.183594 11.183594-2.132812l132.664062-132.828125c7.816406-7.824219 7.816406-20.554688 0-28.378907l-132.664062-132.824218c-4.3125-4.316406-9.257813-2.933594-11.179688-2.136719-1.894531.785156-6.296875 3.253906-6.296875 9.246094v120.902343c0 22.058594-17.945312 40.003907-40.003906 40.003907h-256.015625c-11.046875 0-20-8.953125-20-20s8.953125-20.003907 20-20.003907h256.015625v-120.902343c0-20.273438 12.167969-38.414063 31-46.207031 18.898437-7.820313 40.402344-3.570313 54.78125 10.828124l132.664063 132.824219c23.382812 23.414063 23.382812 61.507813 0 84.921875l-132.664063 132.824219c-9.59375 9.605469-22.359375 14.691406-35.40625 14.695313zm0 0"
              />
            </svg>
          </div>
        </div>
      </div>
      <div>
        <img src="../static/images/about_image.jpg" class="" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
</style>