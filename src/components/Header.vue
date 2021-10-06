<template>
  <div id="Header" class="fluid-container">
    <HeaderSection1 />
    <HeaderSection2 />
  </div>
</template>

<script>
import HeaderSection1 from '../components/HeaderSection1.vue';
import HeaderSection2 from '../components/HeaderSection2.vue';

export default {
    name :"Header",
    components: {
        HeaderSection1,
        HeaderSection2,
  },
}
</script>

<style lang="scss" scoped>

</style>