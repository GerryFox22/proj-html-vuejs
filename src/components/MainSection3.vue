<template>
  <div id="main-section-3">
     <div class="container">
         <div class="row align-items-end">
             <div class="col-6 text-center">
                 <img class="mb-3" src="../assets/images/artist-quote-icon.png" alt="immagine virgolette">
                 <h1 class="fw-bold">I coach and mentor <br>
                    visual artists, like <br>
                    you,to Create Like <br>
                    You Mean It
                 </h1>
                 <h2>Martin Garrix</h2>
             </div>
             <div class="col-6">

                 <p>As a coach and mentor, my ultimate goal is to motivate visual artists <br>
                    toward inspired action. I helo you get you back on track to being the <br>
                    productive, creative, meaningful and authentic artist you truly want <br>
                    to be.I support artists in crafting and living a creative life as well as <br>
                    feeling good about themselves and their art.
                 </p>

                 <p>As an artist and an educator for nearly 30 years, I understand what it <br>
                    takes to create.
                 </p>
                 
                <button class="bottone">Get started today</button>
             </div>
         </div>
     </div>
  </div>
</template>

<script>
export default {
    name : "MainSection3",
}
</script>

<style lang="scss" scoped>
@import "../style/variabili.scss";
#main-section-3 {
    margin-bottom: 150px;
}
h2 {
    font-family: 'Bonheur Royale';
    color: $ccMalibu;
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
</style>