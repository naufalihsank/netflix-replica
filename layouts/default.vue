<template>
  <div>
    <Navbar />
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
import Navbar from './Navbar.vue'
import Footer from './Footer.vue'

export default {
  components: {
    Navbar,
    Footer
  }
}
</script>

<style lang="scss">
body {
  background: #141414;
}
</style>
