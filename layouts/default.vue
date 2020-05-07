<template>
  <div>
    <!-- <Navbar /> -->
    <NavBar2 />
    <nuxt />
  </div>
</template>
<script>
import Navbar from '~/components/Navbar'
import NavBar2 from '~/components/NavBar2'
export default {
  components: {
    Navbar,
    NavBar2
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
