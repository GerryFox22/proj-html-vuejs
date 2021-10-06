<template>
  <div class="hello">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from '../components/Header.vue';
import Main from '../components/Main.vue';
import Footer from '../components/Footer.vue';

export default {
  name: 'PaginaCompleta',
   components: {
    Header,
    Main,
    Footer
  },
  props: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
