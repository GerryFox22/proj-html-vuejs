<template>
  <div id="footer-head">
      <img class="img-1" src="../assets/images/artist-shape-color-paint-top-left.png" alt="immagine sinistra footer">
      <img class="img-2" src="../assets/images/artist-shape-color-paint-bottom-right.png" alt="immagine sinistra footer">
      <div class="container p-5">
          <div class="row justify-content-between align-items-center">
              <div class="col-3">
                  <h2 class="text-white">Newsletter to get <br>
                    in touch
                  </h2>
              </div>
              <div class="email-form col-8">
                  <input class="input-email" type="text" placeholder="Your e-mail">
                  <button class="send-email"><i class="fas fa-long-arrow-alt-right"></i></button>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name : "FooterHead",
}
</script>

<style lang="scss" scoped>

#footer-head{
    background-color: #091fef;
    position: relative;
    .img-1,
    .img-2 {
        position: absolute;
        height: 100%;
    }
    .img-2 {
        right: 0;
    }
}
h2{
    text-align: right;
}

.input-email,
 .send-email{
    background-color: transparent;
    border: none;
    color: white;
    border-bottom: 1px solid gray;
    
}



.input-email {
    width: 80%;
}
 
</style>