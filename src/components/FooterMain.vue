<template>
  <div id="footer-main" class="pt-5 pb-5">
      <div class="container">
          <div class="row">
              <div class="col-3">
                  <h5 class="fw-bold pb-2">Address</h5>
                  <p class="info-indirizzi"> {{indirizzo}} </p>
                  <p class="info-indirizzi"> {{numero}} </p>
                  <p class="info-indirizzi"> {{email}} </p>
                  <div class="socials">
                    <a v-for="(social,indice) in socials" :key="indice" :href="social.link">
                      <i :class="social.icona"></i>
                    </a>
                  </div>
              </div>
              <div class="col-3 ps-5">
                  <h5 class="fw-bold">Explore</h5>
                  <ul>
                    <li v-for="(elemento,indice) in esplora" :key="indice">
                      <a href="#"> {{elemento}} </a>
                    </li>
                  </ul>
              </div>
              <div class="col-3">
                  <h5 class="fw-bold">Information</h5>
                  <ul>
                    <li v-for="(elemento,indice) in informazioni" :key="indice">
                      <a href="#"> {{elemento}} </a>
                    </li>
                  </ul>
              </div>
              <div class="col-3">
                  <span class="fw-bold">Instagram</span><span> <a class="instagram-link" href="#">{{instagramLink}}</a> </span>
                  <div class="post-container d-flex mt-4">
                    <div v-for="(post,indice) in instagramPosts" :key="indice" class="post-singolo">
                      <img :src="post.immagine" :alt="post.alt">
                    </div>
                  </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
  name : "FooterMain",
  data : function (){
    return {
      indirizzo: "382 NE 191st ST # 87349 Miamo, FL 33179-3899",
      numero: "+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)",
      email : "support@maxcoach.com",
      socials : [
              {
                icona :"fab fa-facebook-f",
                link: "#facebook"
              },
              {
                icona :"fab fa-twitter",
                link: "#twitter"
              },
              
              {
                icona :"fab fa-instagram",
                link: "#instagram"
              },
              {
                icona :"fab fa-invision",
                link: "#invision"
              },
            ],
      esplora : ["Start here" ,"Success story","Blog","Courses","Contact us"],
      informazioni :["Membership","Purchase guide","Privacy policy","Terms of services"],
      instagramLink :"@maxcoach" ,
      instagramPosts : [
          {
            immagine : "img/120084500_197897808368764_8114555493043279565_n.jpg",
            alt :"Instagram foto"
          },
          {
            immagine : "img/120012142_177596140500760_8623485824101406058_n.jpg",
            alt :"Instagram foto"
          },
          {
            immagine : "img/120099363_364334431619755_7198812647386067017_n.jpg",
            alt :"Instagram foto"
          },
      ]
    }
  },
}
</script>

<style lang="scss" scoped>

a{
  color: gray;
  font-size: .9rem;
  text-decoration: none;
  padding-right: 35px;
}


.info-indirizzi {
  font-size: .65rem;
}

i{
  font-size: 1.5rem;
}

ul {
  line-height: 30px;
  padding: 0;
  list-style: none;
}

.post-singolo {
  padding-right: 20px;
  img{
    width: 150px;
    height: 150px;
  }
}

.instagram-link{
  color: orange;
}
</style>