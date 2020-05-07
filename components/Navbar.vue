<template>
  <div class="lg:flex lg:justify-between lg:flex-1 lg:items-center bg-blue-800">
    <div class="flex justify-between">
      <nuxt-link to="/">
        <img
          src="@/assets/logo.png"
          alt="Logo mi profe en linea"
        />
      </nuxt-link>
      <span @click="showMenu()">
        <font-awesome-icon
          :icon="['fa', 'bars']"
          class="text-white lg:hidden mr-4 mt-2 mb-2 text-2xl cursor-pointer"
        />
      </span>
    </div>
    <div id="menu" class="hidden lg:block">
      <ul class="lg:flex lg:justify-around">
        <li class="lg:ml-3">
          <nuxt-link to="/">Inicio</nuxt-link>
        </li>
        <li class="lg:ml-3">
          <nuxt-link to="/">¿Quienés Somos?</nuxt-link>
        </li>
        <li class="lg:ml-3">
          <nuxt-link to="/">Servicios</nuxt-link>
        </li>
        <li class="lg:ml-3">
          <nuxt-link to="/">Contacto</nuxt-link>
        </li>
        <li class="lg:ml-3 lg:mr-4">
          <nuxt-link to="/">Login</nuxt-link>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
  methods: {
    showMenu() {
      const menu = window.document.getElementById('menu')
      menu.classList.toggle('is-active')
    }
  }
}
</script>
<style scoped>
img {
  margin-left: 1rem;
  height: 40px;
}
li {
  padding: 0.2rem 0.4rem 0.2rem 1rem;
  color: white;
}
li:hover {
  /* background-color: white; */
  color: yellow;
}
ul {
  margin: 0;
}
@media (max-width: 768px) {
  #menu.is-active {
    display: block;
    transition: max-height 4s;
    max-height: 200px;
  }
}
</style>
