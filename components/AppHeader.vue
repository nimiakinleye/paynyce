<template>
  <div class="">
    <div class="fixed z-50 px-16 py-3 flex items-center justify-between w-full bg-blur shadow-lg">
      <div>
        <LogoIcon />
      </div>
      <div class="text-white self">
        <nuxt-link to="/">Home</nuxt-link>
        <nuxt-link class="ml-12" to="/">About</nuxt-link>
        <nuxt-link class="ml-12" to="/">Subsidiaries</nuxt-link>
        <nuxt-link class="ml-12 my-bg px-6 py-2 rounded" to="/">Lets Talk</nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
import LogoIcon from './LogoIcon'
export default {
  components: {
    LogoIcon
  }
}
</script>

<style>
.bg-blur {
  background: rgb(0, 0, 0, 0.6);
  backdrop-filter: blur(2px);
}
</style>