<template>
  <div class="main">
    <MainJumbo />
    <MainSection2 />
  </div>
</template>

<script>
import MainJumbo from '../components/MainJumbo.vue';
import MainSection2 from '../components/MainSection2.vue';
export default {
  name :"Main",
  components : {
    MainJumbo,
    MainSection2,
  }
}
</script>

<style>

</style>