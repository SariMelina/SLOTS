<template>
  <div class="container">
    <div class="jumbotron">   
      <button class="btn btn-primary"
      @click="componenteSeleccionado='LogIn'">Iniciar Sesión</button>
      <button class="btn btn-primary"
      @click="componenteSeleccionado='ChangePass'">Cambiar Contraseña</button>
      <keep-alive>
        <component v-bind:is="componenteSeleccionado"></component>
      </keep-alive>
    </div>
  </div>
</template>

<script>
import ShowForm from './components/ShowForm.components'
import LogIn from './components/LogIn.component'
import ChangePass from './components/ChangePass.coponents'

export default {
  components: {
    ShowForm,
    LogIn,
    ChangePass
  },
  data() {
    return {
      componenteSeleccionado: 'LogIn'
    }
  }
}
</script>

<style>
  h3{
    color:green
  }
</style>
