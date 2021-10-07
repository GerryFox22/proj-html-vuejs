<template>
  <div id="main-section-7" class="pt-5 pb-5">
      <div class="container">
            <div class="row text-center">
                <h1>Upcoming Events</h1>
            </div>
            <div class="row text-center">
                <h3 class="fw-bold mb-5">Let's Work Togheter</h3>
            </div>
            <div class="row mt-3">
                <div v-for="(evento,indice) in eventi" :key="indice" :class="{inverso : evento.ordineInvertito}"
                class="col-6 d-flex mb-5 align-items-center">
                    <div class="immagine-evento">
                        <img :src="evento.immagine" :alt="evento.alt">
                    </div>
                    <div class="dettagli-evento">
                        <p class="testo-gray"> {{ evento.data }} </p>
                        <h4 class="fw-bold mb-4"> {{ evento.nome }} </h4>
                        <span class="testo-gray">
                            <i class="fas fa-map-marker-alt"> {{ evento.luogo }} </i>
                        </span>
                    </div>
                </div>
            </div>
      </div>
  </div>
</template>

<script>
export default {
    name :"MainSection8",
    data : function (){
        return {
            eventi : [
                {
                    immagine : "img/artist-event-04-250x300.jpg",
                    alt : "immagine evento",
                    data : "NOV 22, 2020",
                    nome : "Storytelling Workshop",
                    luogo : "Texas, US",
                    ordineInvertito : false,
                },
                {
                    immagine : "img/artist-event-03-250x300.jpg",
                    alt : "immagine evento",
                    data : "OCT 10, 2020",
                    nome : "Painting Art Contest 2020",
                    luogo : "New York, US",
                    ordineInvertito : false,
                },
                {
                    immagine : "img/artist-event-02-250x300.jpg",
                    alt : "immagine evento",
                    data : "NOV 23, 2020",
                    nome : "International Art Fair 2020",
                    luogo : "Hamburg, Germany",
                    ordineInvertito : true,
                },
                {
                    immagine : "img/artist-event-01-250x300.jpg",
                    alt : "immagine evento",
                    data : "DEC 15, 2020",
                    nome : "Street Performance: Call for Artist",
                    luogo : "Illinois, US",
                    ordineInvertito : true,
                },
            ],
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

.dettagli-evento{
        margin-left: 40px;
    }

.inverso {
    flex-direction: row-reverse;
    text-align: right;
    .dettagli-evento{
        margin-right: 40px;
    }
}

.testo-gray {
    color: gray;
}
</style>