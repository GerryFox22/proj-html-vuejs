<template>
  <div id="main-section-5" class="mb-5">
      <div class="section5-container pt-5">
          <div class="row text-center">
              <h2>Testimonials</h2>
          </div>
          <div class="row text-center mb-5">
              <h3>Why do people love me?</h3>
          </div>
          <div class="row mb-5">
              <div v-for="(recenzione,indice) in recenzioni" :key="indice" :class="{attivo : recenzione.attivo = true}"
              class=" recensione col p-5">
                  <h4 class="mb-3 fw-bold"> {{ recenzione.titolo }}</h4>
                  <p class="mb-5">{{ recenzione.paragrafo }}</p>
                  <div class="info d-flex">
                      <img class="me-3" :src="recenzione.avatar" :alt="recenzione.alt">
                      <div class="info-persona">
                          <p> <strong> {{ recenzione.nome }} </strong> </p>
                          <p>/ {{ recenzione.ruolo }} </p>
                      </div>
                  </div>
              </div>
          </div>
          <div class="row justify-content-center pb-5">
              <div class="col-3 text-center">
                  <i v-for="(recensione,indice) in recenzioni" :key="indice" class="fas fa-circle"></i>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name : "MainSection5",
    data : function (){
        return {
            recenzioni : [
                {
                    titolo :"It's a choice of quality for people with special needs",
                    paragrafo :"I'm a very strict person so i require everything to be organized and neat. Then,I'll be able to make things right and shine. MaxCpach guys just got me.",
                    avatar :"img/artist-testimonial-avatar-02.jpg",
                    alt :"Florence Themes avatar",
                    nome : "Florence Themes",
                    ruolo: "Multimedia Admin",
                    attivo :false,
                },
                {
                    titolo :"High level of efficiency and scientific teaching methods",
                    paragrafo :"I am free to learn at my ownpace, follow my own schedule and choose the subject i want to learn from the syllabus. Great portal for people like me.",
                    avatar :"img/artist-testimonial-avatar-04.jpg",
                    alt :"Mina Hollace avatar",
                    nome : "Mina Hollace",
                    ruolo: "Freelancer",
                    attivo :true,
                },
                {
                    titolo :"Professional team of specialists and passionate metors at reach",
                    paragrafo :"I need to get a certification for English proficiency and MaxCoach is my best choise. Their tutors are smart and professional when dealing with students",
                    avatar :"img/artist-testimonial-avatar-01.jpg",
                    alt :"Madley Pondor avatar",
                    nome : "Madley Pondor",
                    ruolo: "IT Specialist",
                    attivo :false,
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
@import "../style/variabili.scss";
.section5-container{
    width: 90%;
    margin: 0 auto;
}

h2 {
    font-family: 'Bonheur Royale';
    color: $ccMalibu;
}
.attivo {
    opacity: 1;
}

.recensione {
    background-color: white;
    // opacity: 0.5;
    border: 20px solid $coloreSfondo; 
}

i {
    padding: 10px;
}

.info {
    img {
        width: 60px;
        height: 100%;
        border-radius: 50%;
    }
}
// .non-attivo {
//     // background-color: black;
// }

#main-section-5 {
    background-color: $coloreSfondo;
}
</style>