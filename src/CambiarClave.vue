<template>
  <div class="container">
    <div class="jumbotron">
      <formulario>
        <div slot="titulo">
          <h3 >Recuperar Contraseña</h3>
        </div>
        <div slot="elementos">
          <div class="form-group">
              <label for="correo">Correo Electrónico</label>
              <input type="email" class="form-control"
                  id="correo" placeholder="Escribe tu Correo electrónico">
          </div>
        </div>
        <div slot="boton">
          <button  class="btn btn-primary">Recuperar Contraseña</button>
        </div>
      </formulario>
    </div>
  </div>
</template>



<script>
import Formulario from './MostrarFormulario.vue'
export default {
    components:{
        formulario:Formulario
    },
  data () {
    return{

    }
  }
}
</script>

<style scoped>
</style>
