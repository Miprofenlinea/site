<template>
  <div>
    <div class="back">
      <div class="logo">
        <p class="text-white text-center">Aprende desde cualquier lugar con</p>
        <img
          src="https://miprofenlinea.com/wp-content/uploads/2020/04/3-2.png"
          alt="logo"
        />
        <div class="flex justify-center">
          <Vbutton content="Registrarme" url="/"></Vbutton>
          <Vbutton class="ml" content="Ingresar" url="/"></Vbutton>
        </div>
      </div>
    </div>
    <div class="back-opacity"></div>
  </div>
</template>
<script>
import Vbutton from '~/components/Vbutton'
export default {
  components: {
    Vbutton
  }
}
</script>
<style scoped>
.back {
  background-image: url('https://miprofenlinea.com/wp-content/uploads/2020/04/artificial-intelligence-machine-4082314-1.jpg');
  height: 95vh;
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}
@media (min-width: 769px) {
  .back-opacity {
    position: absolute;
    top: 40px;
    left: 0px;
    width: 100%;
    height: 95vh;
    background-color: Black;
    z-index: 1;
    filter: alpha(opacity=50);
    opacity: 0.5;
  }
  .logo {
    position: absolute;
    z-index: 2;
    margin-left: 15%;
    margin-right: auto;
    margin-top: 25%;
  }
  img {
    display: block;
    margin: auto;
  }
  .ml {
    margin-left: 6rem;
  }
}
</style>
