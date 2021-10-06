<template>
<!-- Nav menu container -->
  <div class="header-navbar d-flex justify-content-between align-items-center">
    <!-- MaxCoach logo -->
      <div class="logo">
        <img src="../assets/images/dark-logo.png" alt="MaxCoach logo">
      </div>
      <!-- Nav menu -->
      <div class="nav-menu">
        <!-- Singoli elementi del nav menu-->
        <ul class="u d-flex">
          <!-- Ciclo for utilizzato sul data Elementi navbar -->
          <li v-for="(elemento, indice) in elementiNavbar" :key="indice">{{elemento}} <i class="fas fa-chevron-down"></i></li>
        </ul>
      </div>
      <!-- Socials -->
      <div class="socials">
        <!-- Ciclo for utilizzato sul data Socials -->
        <a v-for="(social,indice) in socials" :key="indice" :href="social.link">
          <i :class="social.icona"></i>
        </a>
      </div>
  </div>
</template>

<script>
export default {
  name : "HeaderSection2",
   data : function(){
      return {
        // Elementi Navbar
          elementiNavbar : ["Home", "Pages", "Courses", "Features", "Blog", "Shop"],
          // Socials
          socials : [
              {
                icona :"fab fa-twitter",
                link: "#twitter"
              },
              {
                icona :"fab fa-facebook-f",
                link: "#facebook"
              },
              {
                icona :"fab fa-instagram",
                link: "#instagram"
              },
              {
                icona :"fab fa-invision",
                link: "#invision"
              },
          ]
      }
  },
}
</script>

<style lang="scss" scoped>
@import "../style/variabili.scss";
  .header-navbar {
      width: 80%;
      margin: 0 auto;
    }   

   .logo img {
     width: 150px;
   }

   ul {
     list-style: none;
     padding: 0;
     margin: 0;
        li{
          padding: 20px;
           i {
             font-size: 0.8rem;
             cursor: pointer;
           }
        }
   }

   a {
     padding: 10px;
     color: $ccBoulder,
   }
   
   a:hover {
     color: $ccCerulean;
   }

</style>