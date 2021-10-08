<template>
  <div class="footer">
    <FooterHead />
    <FooterMain />
    <FooterEnd />
  </div>
</template>

<script>
import FooterHead from '../components/FooterHead.vue';
import FooterMain from '../components/FooterMain.vue';
import FooterEnd from '../components/FooterEnd.vue';
export default {
  name :"Footer",
  components : {
    FooterHead,
    FooterMain,
    FooterEnd
  }
}
</script>

<style lang="scss" scoped>

</style>