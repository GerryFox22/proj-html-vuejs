<template>
  <div id="main-section-4" class="mb-5">
      <div class="container">
          <img class="img-1" src="../assets/images/maxcoach-shape-05.png" alt="img-1">
          <img class="img-2" src="../assets/images/maxcoach-shape-12.png" alt="img-2">
          <i class="far fa-circle"></i>
          <div class="row justify-content-center p-5">
              <div class="video-container col-9">
                  <button><img src="../assets/images/icon-youtube-play.png" alt=""></button>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name :"MainSection4",
}
</script>

<style lang="scss" scoped>
.video-container {
    position: relative;
    height: 570px;
    background-image: url("../assets/images/artist-video-poster.jpg");
}

.container {
    position: relative;
    .img-1,
    .img-2,
    i{
        position: absolute;
    }
    .img-1{
        left: 13%;
        top: 5%;
    }
    .img-2{
        bottom: 5%;
        left: 80%;
    }
    i{
        z-index: 1;
        font-size: 7rem;
        color: #c09b65;
        left: 82%;
        top: 25%;
    }
}

button {
    background-color: transparent;
    border: 0;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
</style>