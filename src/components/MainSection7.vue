<template>
  <div id="main-section-7" class="pt-5 pb-5">
      <div class="immagini-background">
          <img class="img-1" src="../assets/images/maxcoach-shape-05.png" alt="img-1">
          <i class="far fa-circle background-circle"></i>
          <div class="container">
                <div class="row text-center">
                    <h1>Articles and Tips</h1>
                </div>
                <div class="row text-center">
                    <h3 class="fw-bold mb-5">Latest From The Blog</h3>
                </div>
                <div class="container-immagini">
                    <div class="immagine-piccola sinistra">
                        <div class="immagine-container mb-2">
                            <img src="../assets/images/artist-blog-03-480x356.jpeg" alt="">
                        </div>

                        <div class="info-container p-4">
                            <p class="testo-gray">ARTIST</p>
                            <h5 class="fw-bold mb-4">Brush Stokes Energize <br>
                                Trees in Paintings
                            </h5 >
                            <span class="me-4 testo-gray">
                                <i class="far fa-calendar"></i> May 15, 2020
                            </span>
                            <span class="testo-gray">
                                <i class="far fa-eye"></i> 688 views
                            </span>
                        </div>
                    
                    </div>
                    <div class="immagine-grande d-flex flex-column-reverse p-3">
                        <div class="info-container-grande p-4">
                            <p class="text-white">ARTIST</p>
                            <h2 class="fw-bold text-white mb-4">Connection Between Self- <br>
                                Portraits and Identity
                            </h2>
                            <span class="me-4 text-white">
                                <i class="far fa-calendar"></i> May 15, 2020
                            </span>
                            <span class="text-white">
                                <i class="far fa-eye"></i> 397 views
                            </span>
                        </div>
                    </div>

                    <div class="immagine-piccola destra">
                        <div class="immagine-container mb-2">
                            <img src="../assets/images/artist-blog-01-480x356.jpg" alt="">
                        </div>

                        <div class="info-container p-4">
                            <p class="testo-gray">ARTIST</p>
                            <h5 class="fw-bold mb-4">Pocket-Sinized Notebooks <br>
                                Hold Miniature Paintings
                            </h5>
                            <span class="me-4 testo-gray">
                                <i class="far fa-calendar"></i> May 15, 2020
                            </span>
                            <span class="testo-gray">
                                <i class="far fa-eye"></i> 603 views
                            </span>
                        </div>
                    </div>
                </div>
                <div class="row text-center">
                    <p class="testo-gray"> Get into details now? 
                        <a href="#">View all posts <i class="fas fa-long-arrow-alt-right"></i></a>
                    </p>
                </div>
            </div>
      </div>
      
  </div>
</template>

<script>
export default {
    name :"MainSection7",
}
</script>

<style lang="scss" scoped>
@import "../style/variabili.scss";

h1{
    font-family: 'Bonheur Royale';
    color: $ccMalibu;
}

.immagine-piccola {
    width: 300px;
    position: absolute;
}


.container-immagini {
    position: relative;
    height: 800px;
}

a {
    color: orange;
    text-decoration: none;
}

.background-circle{
    font-size: 7rem;
    color: #c09b65;
}

.immagini-background{
    position: relative;
    background-image: url("../assets/images/maxcoach-shape-03.png");
    background-repeat: no-repeat;
    background-position: center;
    .img-1,
    .background-circle {
        position: absolute;
    }
    .img-1 {
        width: 200px;
        left: 34%;
        top: 18%;
    }
    .background-circle {
        top: 18%;
        left: 13%;
    }
}

.immagine-grande {
    background-image: url("../assets/images/artist-blog-02-500x680.jpg");
    height: 680px;
    width: 500px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.immagine-piccola.sinistra {
    top: 28%;
    left: 2%;
}

.immagine-piccola.destra {
    left: 75%;
    top: 15%;
}

.info-container{
    background-color: white;
}

img {
    width: 300px;

}

p {
    margin-bottom: 10px;
}

.testo-gray{
    color: gray;
}

#main-section-7 {
    background-color: #F5F7FA;
}
</style>