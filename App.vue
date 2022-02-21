<template>
  <div id="app">
    <!--img alt="Vue logo" src="./assets/logo.png"-->
    <!--HelloWorld msg="Welcome to Your Vue.js App"/-->
    <ConvertirMasa/>
    <ConvertirTiempo/>
    <ConvertirMonedas/>
    <ConvertirLongitud/>
    <ConvertirAlmacenamiento/>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import ConvertirMasa from './components/ConvertirMasa.vue'
import ConvertirTiempo from './components/ConvertirTiempo.vue'
import ConvertirMonedas from './components/ConvertirMonedas.vue'
import ConvertirLongitud from './components/ConvertirLongitud.vue'
import ConvertirAlmacenamiento from './components/ConvertirAlmacenamiento.vue'
export default {
  name: 'App',
  components: {
    //HelloWorld,
    ConvertirMasa,
    ConvertirTiempo,
    ConvertirMonedas,
    ConvertirLongitud,
    ConvertirAlmacenamiento
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
