<template>
  <div>
    <section>
      
      <div class="back">
        <div class="back-opacity">
          <div class="logo">
        <div>
          <p class="text-white text-center Euphoria">
            Aprende desde cualquier lugar con
          </p>
        </div>

          <div class="flex justify-center">
            <img src="@/assets/logo.png" alt="logo" />
          </div>

          <div class="mt">
            <div class="flex justify-center">
              <Vbutton class=".boton" content="Registrarme" url="/"></Vbutton>
              <Vbutton class="ml" content="Ingresar" url="/"></Vbutton>
            </div>
          </div>
        </div>
        </div>
      </div>
    </section>


    
    
    <section class="justify-center secH">

      <div class="redes">

      </div>

      <div class="caja1">
        <p>¿Qué quieres hacer hoy?</p>
        
      </div>

      <div class="caja2" >
      <yoQuiero  content="Encuentra el profe ideal para ti" vContent="Aprender" uImage="@/components/aprender.PNG" url="/"></yoQuiero>
      </div>
      <div class="caja2">
      <yoQuiero  content="Se el gran profesor que tus alumnos necesitan. " vContent="Aprender" uImage="@/components/aprender.PNG" url="/"></yoQuiero>
      </div>
    </section>

  </div>
</template>
<script>
import Vbutton from '~/components/Vbutton'
import YoQuiero from '~/components/YoQuiero'

export default {
  components: {
    Vbutton,
    YoQuiero

  }
}
// 

</script>
<style scoped>
.redes{
  width: 100%;
  margin-top: 15px;
  padding-top: 10px;
  border: 1px solid black;
  align-items: center;

}

.caja1{
  width: 100%;
  margin-top: 15px;
  padding-top: 10px;
  border: 1px solid blue;

}

.caja1 p{
  color: #000;
  font-family: Euphoria;
  font-weight: 100;
  font-size: 50px;
  letter-spacing: 2px;
  text-align: center;
  border: 1px solid green;
}



.caja2{
  width: 47.5%;
  display: inline-block;
  margin: 1%;
}


.back {
  background: url('https://miprofenlinea.com/wp-content/uploads/2020/04/artificial-intelligence-machine-4082314-1.jpg');
  height: 95vh;
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  background-attachment: fixed;

  
}
/* esto es para computador */
.back-opacity {
  left: 0px;
  width: 100%;
  height: 95vh;
  background-color:rgba(4, 2, 25, 0.55);
  /* filter: brightness(100%) contrast(80%) saturate(1.02); */



}
.logo {
  position: absolute;
  width: 100%;
  margin-top: 16%;
  height: 95vh;
}
img {
  display: block;
  margin-top: 20px;
  width: 30%;
}
.ml {
  margin-left: 6rem;
}
.mt {
  margin-top: 20px;
}

.boton {
  font-size: 16px;
}
.boton:hover{
  font-size: 18px;
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
@media (max-width: 907px) {
  .logo {
  margin-top: 20%;
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

@media (max-width: 430px){
  .caja2{
  width: 100%;
  display: inline-block;
  margin: 1%;
}

}
</style>
