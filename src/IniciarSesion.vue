<template>
  <div  class="container">
    <div class="jumbotron">
      <formulario>
        <div slot="titulo">
          <h3 >Iniciar Sesión</h3>
        </div>
        <div slot="elementos">
          <div class="form-group">
              <label for="correo">Correo Electrónico</label>
              <input type="email" class="form-control"
                  id="correo" placeholder="Escribe tu Correo electrónico">
          </div>    
          <div class="form-group">
              <label for="clave">Contraseña</label>
              <input type="password" name="clave" id="clave"
                  class="form-control" placeholder="Escribe tu contraseña">
          </div>
        </div>
        <div slot="boton">
          <button  class="btn btn-primary">Iniciar Sesión</button>
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
