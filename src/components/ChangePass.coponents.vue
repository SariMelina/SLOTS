<template>
  <div class="container">
    <div class="jumbotron">   
      <ShowForm>
        <div slot="titulo">
           <h3>Cambiar Contraseña</h3>
        </div>
        <div slot="correo">
          <div class="form-group">
            <label for="correo">Correo Electrónico</label>
            <input type="email" class="form-control" id="correo"
            placeholder="example@hotmail.com">
          </div>
          <div class="form-group">
            <label for="clave">Contraseña</label>
            <input type="password" class="form-control"
            id="clave" placeholder="Escribe tu contraseña">
          </div>
        </div>
        <div slot="boton">
          <button class="btn btn-primary">Iniciar Sesión</button>
        </div>
      </ShowForm>
    </div>
  </div>
</template>

<script>
import ShowForm from './ShowForm.components'

export default {
  components: {
    ShowForm
  }
}
</script>

<style>
  h3{
    color:green
  }
</style>
