<template>
  <div class="py-2 px-12 lg:px-48">
    <div class="flex flex-col md:flex-row justify-between my-20">
      <div class="mb-8">
        <div>
          <img class="w-10" src="~/assets/logo.png" alt="">
          NimiAkinleye
        </div>
        <div class="flex items-end md:justify-between">
          <nuxt-link to="/" class="mr-3">
            <svg
              class="w-5 fill-current"
              viewBox="0 0 40 40"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g opacity="0.7">
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M8.3908 40V13.5464H0.251119V40H8.3908ZM8.3908 4.16977C8.34231 1.80245 6.77161 0 4.21997 0C1.66767 0 0 1.80245 0 4.16977C0 6.48568 1.61918 8.34026 4.12234 8.34026H4.17082C6.77161 8.34026 8.3908 6.48568 8.3908 4.16977ZM21.6702 40V24.928C21.6702 24.1214 21.7283 23.3148 21.9644 22.7397C22.61 21.1273 24.0793 19.4581 26.5464 19.4581C29.7785 19.4581 31.8054 21.3006 31.8054 24.928V40H40V24.5247C40 16.2348 35.5945 12.3774 29.718 12.3774C24.8998 12.3774 22.7849 15.0832 21.6106 16.9248L21.6694 13.3868H13.489C13.6067 15.9193 13.489 40 13.489 40H21.6702Z"
                  fill="currentColor"
                />
              </g>
            </svg>
          </nuxt-link>
          <nuxt-link to="/" class="mr-3">
            <svg
              class="w-6 fill-current"
              viewBox="0 0 50 40"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                opacity="0.7"
                d="M49.2212 4.73497C47.4117 5.53929 45.4644 6.08183 43.4211 6.32462C45.5073 5.07569 47.107 3.09737 47.8613 0.737373C45.91 1.89539 43.7498 2.73567 41.4488 3.18929C39.6073 1.22696 36.9826 0 34.078 0C28.5018 0 23.9806 4.52116 23.9806 10.0984C23.9806 10.8887 24.0695 11.6591 24.2424 12.3995C15.8495 11.9778 8.40785 7.95823 3.42709 1.84843C2.55783 3.33916 2.06025 5.07369 2.06025 6.92611C2.06025 10.4291 3.84273 13.5205 6.55243 15.331C4.89784 15.278 3.34016 14.8234 1.97832 14.067C1.97732 14.109 1.97732 14.152 1.97732 14.1949C1.97732 19.0868 5.45836 23.1673 10.0784 24.0965C9.23115 24.3263 8.33891 24.4502 7.4177 24.4502C6.76625 24.4502 6.13379 24.3873 5.51731 24.2684C6.80322 28.28 10.532 31.2005 14.9503 31.2814C11.4942 33.9901 7.14093 35.6047 2.40895 35.6047C1.59464 35.6047 0.790328 35.5568 0 35.4629C4.4702 38.3294 9.77769 40 15.4798 40C34.0551 40 44.2114 24.6131 44.2114 11.2684C44.2114 10.8308 44.2024 10.3942 44.1834 9.96053C46.1558 8.53974 47.8683 6.76025 49.2212 4.73497Z"
                fill="currentColor"
              />
            </svg>
          </nuxt-link>
          <nuxt-link to="/">
            <svg
              class="w-3 fill-current"
              viewBox="0 0 21 40"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g opacity="0.7">
                <path
                  d="M13.4831 40V21.7555H19.6046L20.523 14.6431H13.4831V10.1029C13.4831 8.0444 14.0524 6.64153 17.0077 6.64153L20.7708 6.63998V0.27846C20.12 0.193891 17.8862 0 15.2862 0C9.85697 0 6.14004 3.31393 6.14004 9.39854V14.6431H0V21.7555H6.14004V40H13.4831Z"
                  fill="currentColor"
                />
              </g>
            </svg>
          </nuxt-link>
        </div>
      </div>
      <div class="mb-8">
        <div class="font-semibold mb-2">Location</div>
        <div>982 S Front St. Columbus, OH 43206</div>
      </div>
      <div>
        <div class="font-semibold mb-2">Enquiries</div>
        <div>+234 708 506 2512</div>
        <div>toluwanimiakinleye01@gmail.com</div>
      </div>
    </div>
    <div class="border-t-2 border-gray-300">
      <div class="flex flex-col md:flex-row items-center justify-between pt-2">
        <div class="flex divide-x divide-gray-200 mb-3">
          <nuxt-link to="/" class="px-4">Privacy Policy</nuxt-link>
          <nuxt-link to="/" class="px-4">Legal</nuxt-link>
          <nuxt-link to="/" class="px-4">News</nuxt-link>
        </div>
        <div>
          Copyright 2021 - NimiAkinleye
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from './Logo'
export default {
  components: {
    Logo,
  },
}
</script>

<style>
</style>