<template>
  <div class="jumbo d-flex">
      <div class="col-6 conternitore-sinistro">
          <img class="img-1" src="../assets/images/artist-hero-image-02-232x300.jpg" alt="">
          <img class="img-2" src="../assets/images/artist-hero-image-01.jpg" alt="">
          <img class="img-3" src="../assets/images/artist-hero-image-03-204x300.png" alt="">
          <img class="img-4" src="../assets/images/artist-shape-03.png" alt="">
      </div>
      <div class="testo text-center">
          <h1>Hello, Im Martin</h1>
          <h3 class="mb-4">Artist Coaching And Mentoring <br>
            Might Be for You.
          </h3>
          <button class="bottone">Get started today</button>
      </div>
      <div class="col-6 contenitore-destro">
          <img class="img-1" src="../assets/images/artist-hero-image-04-235x300.jpg" alt="">
          <img class="img-2" src="../assets/images/artist-shape-05-300x198.png" alt="">
          <img class="img-3" src="../assets/images/artist-shape-04-127x300.png" alt="">
      </div>
  </div>
</template>

<script>

export default {

}
</script>

<style lang="scss" scoped>
@import "../style/variabili.scss";
    .jumbo {
        background-color: $coloreSfondo;
        height: 500px;
        position: relative;
        .testo{
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);

            h1{
                font-family: 'Bonheur Royale';
                color: $ccMalibu;
            }
            h2 {
                font-weight: 800;
            }

            .bottone{
                color: white;
                background-color: $ccThunderbird;
                border: 0;
                padding: 10px 25px;
                border-radius: 5px;
                &:hover {
                    background-color: $ccCerulean;
                }
            }
        }
    }

    .conternitore-sinistro {
        position: relative;
        background-image: url("../assets/images/artist-shape-02-300x162.png");
        background-position: top;
        background-repeat: no-repeat;
        background-size: contain;
        .img-1 {
            z-index: 3;
            width: 200px;
            left: 36%;
            top: 13%;
        }
        .img-2 {
            z-index: 4;
            width: 130px;
            bottom: 9%;
            left: 20%;
        }
        .img-3 {
            z-index: 2;
            width: 150px;
            bottom: 3%;
            left: 50%;
        }
        .img-4 {
            width: 230px;
            z-index: 1;
            bottom: 10%;
            left: 8%;
        }
        
    }

    .contenitore-destro {
        position: relative;
        background-image: url("../assets/images/artist-shape-01-600x577.png");
        background-position: center;
        background-repeat: no-repeat;
        background-size: contain;
        .img-1 {
            position: absolute;
            z-index: 1;
            bottom: 7%;
            left: 45%;
        }
        .img-2 {
            position: absolute;
            bottom: 0;
            left: 53%;
        }
        .img-3 {
            width: 100px;
            position: absolute;
            left: 71%;
            top: 9%;

        }
    }

    img{
        position: absolute;
    }
</style>