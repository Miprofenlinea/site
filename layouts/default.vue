<template>
  <div>
    <Navbar />
    <nuxt />
  </div>
</template>
<script>
import Navbar from '~/components/Navbar'
export default {
  components: {
    Navbar
  }
}
</script>
<style>
*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
</style>
