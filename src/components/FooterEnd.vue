<template>
  <div id="footer-end">
      <div class="container">
        <div class="row text-center p-5">
          <span class="text-gray">@ 2020 Maxcoeach. All Rights Reserved</span>
        </div>
        <button> <i class="fas fa-long-arrow-alt-up"></i> </button>
      </div>
  </div>
</template>

<script>
export default {
  name :"FooterEnd",
}
</script>

<style lang="scss" scoped>

.text-gray{
  color: gray;
  font-size: .7rem;
}

#footer-end{
  position: relative;
  button {
    position: absolute;
    right: 4%;
    bottom: 20%;
    color: white;
    border: 0;
    background-color: orange;
    border-radius: 50%;
    height: 50px;
    width: 50px;

  }
}
</style>