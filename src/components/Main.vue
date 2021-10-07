<template>
  <div class="main">
    <MainJumbo />
    <MainSection2 />
    <MainSection3 />
    <MainSection4 />
    <MainSection5 />
    <MainSection6 />
    <MainSection7 />
  </div>
</template>

<script>
import MainJumbo from '../components/MainJumbo.vue';
import MainSection2 from '../components/MainSection2.vue';
import MainSection3 from '../components/MainSection3.vue';
import MainSection4 from '../components/MainSection4.vue';
import MainSection5 from '../components/MainSection5.vue';
import MainSection6 from '../components/MainSection6.vue';
import MainSection7 from '../components/MainSection7.vue';
export default {
  name :"Main",
  components : {
    MainJumbo,
    MainSection2,
    MainSection3,
    MainSection4,
    MainSection5,
    MainSection6,
    MainSection7,
  }
}
</script>

<style>

</style>