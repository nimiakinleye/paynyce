<template>
  <div>
    <AppHeader />
    <Nuxt />
    <AppFooter />
  </div>
</template>


<script>
import AppHeader from '../components/AppHeader'
import AppFooter from '../components/AppFooter'
export default {
  components: {
    AppHeader,
    AppFooter
  }
}
</script>

<style>
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  scroll-behavior: smooth;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.my-color {
  color: #FF350D;
}

.my-bg {
  background-color: #FF350D;
}

.my-bg:hover {
  background-color: rgb(255, 53, 13, 0.8)
}

.my-container {
  @apply mx-auto;
  padding: 0 24px;
}

.my-line {
  @apply h-0.5 w-48
}

.new-page {
  @apply mt-32
}

</style>
