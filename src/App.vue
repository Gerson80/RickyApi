<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import Titulo from './components/Titulo.vue'
import Inicio from './components/Inicio.vue'
import Navegacion from './components/Navegacion.vue'
import Personajes from './components/Personajes.vue'

</script>

<template>

 

  <header>

    <div>
      <Titulo msg="Rick and Morty" />
      <Navegacion></Navegacion>



    </div>
  </header>
  

  <RouterView />
</template>


