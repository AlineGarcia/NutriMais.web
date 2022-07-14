<template>
  <v-app>
    <div class="app-primary">
      <Cabecalho/>
    </div>
    <Home/>
  </v-app>
</template>

<script>
import Cabecalho from './components/commons/Cabecalho.vue'
import Home from './views/Home.vue'
export default {
  name: 'App',
  components: {
    Cabecalho, 
    Home
  }
}
</script>

<style>
.app-primary {
  height: 80px;
}
</style>
