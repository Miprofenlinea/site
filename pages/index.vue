<template>
  <div>
    <section>
      <div class="back">
        <div class="logo">
          <div>
            <p class="text-white text-center Euphoria">
              Aprende desde cualquier lugar con
            </p>
            <div class="flex justify-center">
              <img
                src="https://miprofenlinea.com/wp-content/uploads/2020/04/3-2.png"
                alt="logo"
              />
            </div>
            <div class="mt">
              <div class="flex justify-center">
                <Vbutton content="Registrarme" url="/"></Vbutton>
                <Vbutton class="ml" content="Ingresar" url="/"></Vbutton>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="back-opacity"></div>
    </section>
    <section class="flex justify-center secH">
      <yoQuiero content="Aprender" url="/"></yoQuiero>
    </section>
  </div>
</template>
<script>
import Vbutton from '~/components/Vbutton'
export default {
  components: {
    Vbutton
  }
}
// import YoQuiero from '~/components/YoQuiero'
</script>
<style scoped>
.back {
  background-image: url('https://miprofenlinea.com/wp-content/uploads/2020/04/artificial-intelligence-machine-4082314-1.jpg');
  height: 95vh;
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  position: relative;
}
/* esto es para computador */
.back-opacity {
  position: absolute;
  top: 40px;
  left: 0px;
  width: 100%;
  height: 95vh;
  background-color: Black;
  z-index: 1;
  filter: alpha(opacity=55);
  /* brightness: 100%;
  contrast: 80%;
  saturate: 102%; */
  opacity: 0.6;
}
.logo {
  position: absolute;
  z-index: 2;
  width: 100%;
  margin-top: 16%;
}
img {
  display: block;
  margin-top: 20px;
  width: 500px;
}
.ml {
  margin-left: 6rem;
}
.mt {
  margin-top: 45px;
}
@font-face {
  src: url(fuentes/EuphoriaScript-Regular.ttf);
  font-family: Euphoria; /*aquí pone el nombre con el que quiera recordarla.*/
}
.Euphoria {
  color: #fff;
  font-family: Euphoria;
  font-weight: 100;
  font-size: 26px;
  letter-spacing: 2px;
}
.secH {
  height: 95vh;
  align-items: center;
}
/* Esto es para celulares */
@media (max-width: 640px) {
  .back-opacity {
    position: absolute;
    top: 40px;
    left: 0px;
    width: 100%;
    height: 95vh;
    background-color: Black;
    z-index: 1;
    filter: alpha(opacity=55);
    opacity: 0.6;
  }
  .logo {
    position: absolute;
    z-index: 2;
    width: 100%;
    margin-top: 50%;
  }
  img {
    display: block;
    margin-top: 20px;
    width: 300px;
  }
  .ml {
    margin-left: 6rem;
  }
  .mt {
    margin-top: 30px;
  }
  @font-face {
    src: url(fuentes/EuphoriaScript-Regular.ttf);
    font-family: Euphoria; /*aquí pone el nombre con el que quiera recordarla.*/
  }
  .Euphoria {
    color: #fff;
    font-family: Euphoria;
    font-weight: 100;
    font-size: 25px;
    letter-spacing: 2px;
  }
}
</style>
