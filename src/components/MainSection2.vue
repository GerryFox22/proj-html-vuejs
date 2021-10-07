<template>
  <div id="main-section-2" class="mb-5">
      <img class="img-1" src="../assets/images/artist-shape-01.png" alt="img-1">
      <img class="img-2" src="../assets/images/maxcoach-shape-13.png" alt="img-1">
    <div class="artist-section-container container align-items-baseline">
        <div class="row text-center">
            <h1>Artist coaching</h1>
        </div>
        <div class="row text-center">
            <h3 class="fw-bold mb-5">I undestand what it takes to create. <br>
                I can help you with
            </h3>
        </div>
        <div class="row">
            <div v-for="(info,indice) in infoCorso" :key="indice" class="col-3">
                <img class="mb-3" :src="info.src" :alt="info.alt">
                <h5 class="mb-3">{{ info.titolo }}</h5>
                <p>{{ info.paragrafo }}</p>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name :"MainSection2",
    data : function(){
        return {
            infoCorso : [
                {
                    src : "img/artist-box-image-01.png",
                    alt : "Corsi online",
                    titolo : "Online Courses",
                    paragrafo : "Online art coaching now offers you a very powerful way to redisign your artist mind."
                },
                {
                    src : "img/artist-box-image-02.png",
                    alt : "One to One",
                    titolo : "One to One",
                    paragrafo : "Getting the necessary clarity about the current state to help you improve your ability."
                },
                {
                    src : "img/artist-box-image-03.png",
                    alt : "Anywhere",
                    titolo : "Anywhere",
                    paragrafo : "Access to valuable and portable program which allow you to setup and live anywhere you want."
                },
                {
                    src : "img/artist-box-image-04.png",
                    alt : "One Time",
                    titolo : "One Time",
                    paragrafo : "Punctuality is our top priority because it's an essential criteria to assess a program quality."
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variabili.scss";

h1{
    font-family: 'Bonheur Royale';
    color: $ccMalibu;
}
p,h5{
    margin: 0;
}
#main-section-2 {
    position: relative;
    background-image: url("../assets/images/maxcoach-shape-14.png");
    background-repeat: no-repeat;
    background-size: contain;
    background-position: center;
    height: 500px;
    .img-1 {
        position: absolute;
        top: 10%;
        width: 500px;
        transform: rotate(220deg);
    }
    .img-2 {
        position: absolute;
        right: 0;
        top: 30%;
    }

}

.artist-section-container {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

</style>