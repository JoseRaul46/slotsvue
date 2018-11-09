<template>
  <div  class="container">
    <div class="jumbotron">
      <button class="btn btn-primary" 
        @click="componenteSeleccionado= 'iniciarSesion'">
        Iniciar Sesión
      </button>    
      <button class="btn btn-primary" 
        @click="componenteSeleccionado= 'cambiarClave'">
        Recuperar Contraseña
      </button>
      <keep-alive>
        <component :is="componenteSeleccionado"></component>
      </keep-alive>
    </div>
  </div>
</template>



<script>
import Formulario from './MostrarFormulario.vue'
import IniciarSesion from './IniciarSesion.vue'
import CambiarClave from './CambiarClave.vue'

export default {
  components:{
    formulario : Formulario,
    iniciarSesion : IniciarSesion,
    cambiarClave : CambiarClave
  },
  data () {
    return{
      componenteSeleccionado:'iniciarSesion'
    }
  }
  
}
</script>

<style scoped>
</style>
