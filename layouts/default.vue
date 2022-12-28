<template>
  <div>
    <Navbar />
    <Nuxt />
  </div>
</template>

<script>
import Navbar from './Navbar.vue'

export default {
  components: {
    Navbar
  }
}
</script>

<style lang="scss">
body {
  background: #521d0e;
}
</style>
