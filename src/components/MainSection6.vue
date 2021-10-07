<template>
  <div id="main-section-6" class="mb-5">
      <div class="container">
        <div class="row text-center">
            <h1>Artist coaching</h1>
        </div>
        <div class="row text-center">
            <h3 class="fw-bold mb-5">Latest Online Courses</h3>
        </div>
        <div class="row">
            <div v-for="(corso,indice) in corsi" :key="indice" class="corso col-3 mb-4">
                <div class="immagine-corso-container">
                    <img :src="corso.immagine" :alt="corso.alt">
                </div>
                <div class="info-corso p-4">
                    <p class="prezzo fw-bold"> {{ corso.prezzo }} </p>
                    <p class="fw-bold"> {{ corso.nome }} </p>
                    <span class="pe-4">
                        <i class="far fa-file-archive"> {{ corso.lezioni }} </i>
                    </span>
                    <span>
                        <i class="far fa-user"> {{ corso.studenti }} </i>
                    </span>
                </div>
            </div>
        </div>
        <div class="row">
            <div class="bottone-container text-center">
                <button class="bottone">View all courses <i class="fas fa-long-arrow-alt-right"></i></button>
            </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name :"MainSection6",
    data : function (){
        return {
            corsi : [
                {
                    immagine : "img/artist-course-08-480x480.jpg",
                    alt : "immagine corso",
                    prezzo : "$18.00",
                    nome : "The Acrylic Painting Academy",
                    lezioni : "4 Lessons",
                    studenti: "50 Students",
                },
                {
                    immagine : "img/artist-course-07-480x480.jpg",
                    alt : "immagine corso",
                    prezzo : "$21.00",
                    nome : "Drawing and Shading: Complete Course",
                    lezioni : "14 Lessons",
                    studenti: "50 Students",
                },
                {
                    immagine : "img/artist-course-06-480x480.jpg",
                    alt : "immagine corso",
                    prezzo : "$19.00",
                    nome : "The Color Theory for Digital Artist",
                    lezioni : "7 Lessons",
                    studenti: "50 Students",
                },
                {
                    immagine : "img/artist-course-05-480x480.jpg",
                    alt : "immagine corso",
                    prezzo : "$35.00",
                    nome : "Ultimate Guide to Digital Sketching for Beginner",
                    lezioni : "14 Lessons",
                    studenti: "50 Students",
                },
                {
                    immagine : "img/artist-course-04-480x480.jpg",
                    alt : "immagine corso",
                    prezzo : "$19.00",
                    nome : "Portrait Drawing The Smart Way",
                    lezioni : "2 Lessons",
                    studenti: "50 Students",
                },
                {
                    immagine : "img/artist-course-03-480x480.jpg",
                    alt : "immagine corso",
                    prezzo : "$19.00",
                    nome : "Mastering Watercolor Painting from Beginner",
                    lezioni : "9 Lessons",
                    studenti: "50 Students",
                },
                {
                    immagine : "img/artist-course-02-480x480.jpg",
                    alt : "immagine corso",
                    prezzo : "$25.00",
                    nome : "The Art & Science of Drawing",
                    lezioni : "4 Lessons",
                    studenti: "50 Students",
                },
                {
                    immagine : "img/artist-course-01-480x480.jpg",
                    alt : "immagine corso",
                    prezzo : "$22.00",
                    nome : "The Colored Pencil Drawing Course",
                    lezioni : "6 Lessons",
                    studenti: "50 Students",
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
@import "../style/variabili.scss";

h1{
    font-family: 'Bonheur Royale';
    color: $ccMalibu;
}

.prezzo {
    color: orange;
}

p {
    font-size: 1.2rem;
}

.corso {
    position: relative;
    cursor: pointer;
}

.corso:hover .info-corso{
    width: 80%;
    border: 3px solid orange;
    background-color: white;
    position: absolute;
    top: 50%;
}

.bottone{
    color: $ccThunderbird;
    background-color:#ffe9c9;
    border: 0;
    padding: 10px 25px;
    border-radius: 5px;
    &:hover {
        color: white;
        background-color: $ccThunderbird;
    }
}

img {
    width: 100%;
}
</style>