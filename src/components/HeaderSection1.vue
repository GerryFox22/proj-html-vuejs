<template>
<!-- Header section 1 container -->
  <div class="header-section-1 d-flex justify-content-center align-items-center p-2">
      <!-- Presentazione offerta -->
      <div class="presentazione-offerta me-4">
          <p>Start TOMORROW! Our biggest event of the year...</p>
      </div>
      <!-- Tempo offerta -->
      <div class="tempo-offerta me-4">
          <i class="far fa-clock"></i>
          <span> <strong> 00 : 00 : 00 </strong> </span>
      </div>
      <!-- Bottone ticket -->
      <div class="bottone-ticket ms-3">
          <button class="bottone">Get Ticket</button>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../style/variabili.scss";
     .header-section-1{
        background-color: lightgray;
    }
    p{
        margin: 0;
    }
    .bottone{
        color: white;
        background-color: $ccThunderbird;
        border: 0;
        padding: 5px 30px;
        border-radius: 10px;
        &:hover {
            background-color: $ccCerulean;
        }
    }
</style>