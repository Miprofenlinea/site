<template>
  <div>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.1/css/all.css" integrity="sha384-50oBUHEmvpQ+1lW4y57PTFmhCaXp0ML5d60M1M7uH2+nqUivzIebhndOJK28anvf" crossorigin="anonymous">

    <header>
            <div class="logo">
                <a href="/"><img src="@/assets/logo.png"></a>
            </div>
            <nav id="menu">
                <ul>
                    <li><a href="/">Inicio</a></li>
                    <li class="align-items-center"><a href="/"><span><img src="@/assets/buscarP.png" class="buscarP"></span>Busca un Profe</a></li>
                    <li><a href="/">¿Quiénes Somos?</a></li>
                    <li><a href="/">Servicios</a></li>
                    <li><a href="/">Contacto</a></li>
                    <li><a href="/">Login</a></li>
                </ul>
            </nav>
            <div class="menu-toggle">
                <i class="fa fa-bars" @click="ToggleClick"></i>
            </div>
        </header>
    </div>
</template>

<script>
export default {
    name: 'NavBar',

    methods:{
        ToggleClick(){ //este metodo cambia las barras del menu por una X
            let menuToggleIcon = document.querySelector('.menu-toggle i');
            let menu = document.getElementById('menu');
            menu.classList.toggle('show');
            if(menu.classList.contains('show')){
                menuToggleIcon.setAttribute('class','fa fa-times');
            }else{
                menuToggleIcon.setAttribute('class','fa fa-bars')
            }
        }
    }
}
</script>

<style scoped>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
.container{
    padding: 50px;
    margin: 50px;
    text-align: justify;
    font-family: 'Lucida Sans';
}
header{
    height: 70px;
    background: rgb(33, 87, 156);
    display: flex;
    padding: 0 20px ;
    box-shadow: 0 2px 5px;
}
.menu-toggle{
    display: none;
    margin-left: auto;
    color: #fff;
    line-height: 70px;
    font-size: 25px;
    cursor: pointer;
}
.logo img{
    line-height: 70px;
    padding-top: 5px;
    height: 60px;
    padding-left: 10px;
    transition: .3s;
}
.logo img:hover{
    height: 65px;
    line-height: 70px;
    padding-top: 0;
    padding-left: 0;
}

      /*---- Mis Elementos del menu---- */

#menu{
    margin-left: auto;
    position: relative;
    z-index: 1;
}
#menu ul li{
    display: inline-block;
}
.buscarP{
    float: left;
    height: 20px;
    padding-right: 5px;
    margin-top: 25px;
}
#menu ul li a{
    display: inline-block;
    position: relative;
    color: #fff;
    text-decoration: none;
    line-height: 70px;
    padding: 0 10px;
    transition: .3s;
    font-family: 'Lucida Sans';
    border-radius: 20px;
    font-size: 16px;
}
#menu ul li a:hover{
    /* background: rgb(45, 114, 204) ;
    margin: 5px;  probar estos dos*/
    color: yellow;

    font-size: 19px;
}
/* -----submenu ????*/

    /* -----OTROS DISPOSITIVOS----- */
.show{
    position: relative;
    z-index: 2;
    height: 450px !important;
}
@media screen and (max-width: 907px){
    .menu-toggle{
        display: block;
        transition: .2s;
        
    }
    .menu-toggle:hover{
        font-size: 30px;
    }
    #menu{
        /* background:  rgb(33, 87, 156); */
        position: absolute;
        top: 50px;
        left: 0;
        width: 100%;
        min-width: 200px;
        height: 0;
        /* border: 1px  solid #fff; */
        overflow: hidden;
        transition: .3s;
        border-radius: 20px;
        margin-top: 30px;
    }
    #menu ul li{
        display: block;
        text-align: center;
    }
    #menu ul li a{
        background:  rgb(33, 87, 156);
        color: #fff;
        font-size: 20px;
        border-bottom: 1px solid #fff;
        width: 100%;
        margin-top: 3px;
        display: inline-block;
    }
    #menu ul li a:hover{
        background:  rgb(79, 115, 161);
    }
    .container{
        padding: 10px;
    }
}
</style>

