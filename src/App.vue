<template>
  <div id="app">
    <!-- Font awesome --> 
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"/>
    
    <PaginaCompleta/>
  </div>
</template>

<script>
import PaginaCompleta from './components/PaginaCompleta.vue'

export default {
  name: 'App',
  components: {
    PaginaCompleta,
  }
}
</script>

<style lang="scss">
@import "style/generali.scss";
@import "style/variabili.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;


}
</style>
