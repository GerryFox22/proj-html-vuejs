<template>
  <div class="main">
    <MainJumbo />
    <MainSection2 />
    <MainSection3 />
  </div>
</template>

<script>
import MainJumbo from '../components/MainJumbo.vue';
import MainSection2 from '../components/MainSection2.vue';
import MainSection3 from '../components/MainSection3.vue';
export default {
  name :"Main",
  components : {
    MainJumbo,
    MainSection2,
    MainSection3,
  }
}
</script>

<style>

</style>