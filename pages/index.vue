<template>
  <div class="index-page">
    <Banner />
    <About id="about"/>
    <Subsidiaries id="subsidiaries"/>
    <ContactUs id="contact-us"/>
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
.index-page {
  transition: 0.5s;
}

</style>
