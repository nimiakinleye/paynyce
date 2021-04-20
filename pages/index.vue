<template>
  <div class="">
    <Banner />
    <About />
    <Subsidiaries />
    <ContactUs />
  </div>
</template>

<script>
import Banner from '../components/Banner'
import About from '../components/About'
import Subsidiaries from '../components/Subsidiaries'
import ContactUs from '../components/ContactUs'
export default {
  components: {
    Banner,
    About,
    Subsidiaries,
    ContactUs
  }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

</style>
