<template>
 <section>
   <div class="hello">
      <div class="image" :style="{ backgroundImage: `url( ${Image} )` }">
        <h1>{{ msg }}</h1>
        <div class="card" style="width: 34rem;">
          <img alt="logo" class="card-img-top" src="../assets/LOGO.png">
          <div class="card-body">
            <h5 class="card-title text-center">Programme de Formation accélérée</h5>
            <p class="card-text text-center">L'intégration des femmes dans les forces de l'ordre <br>est un atout majeur pour le renforcement de la sécurité</p>
            <div class="social">
              <a href="https://web.facebook.com/Pamif-Pnh-107899311596451" target="_blank"><fa :icon="['fab', 'facebook']" /></a>
              <a href="https://twitter.com/PamifP" target="_blank"><fa :icon="['fab', 'twitter']" /></a>
            </div>
          </div>
        </div>
      </div>
    </div>
 </section>
</template>

<script>
import Image from '@/assets/background.png'

export default {
  data: () => ({
    Image
  }),
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.image {
  height: 92vh;;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

.image h1 {
  text-align: center;
  padding-top: 10px;
}

.card {
  margin-left: auto;
  margin-right: auto;
  background-color: rgba( 255, 255, 255, 0.65 );
  border: 1px solid rgba(250, 235, 215, 0.473);
  border-radius: 10px;
  box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
  backdrop-filter: blur( 2.5px );
  -webkit-backdrop-filter: blur( 2.5px );
}

.card img {
  width: 20rem;
  margin-left: auto;
  margin-right: auto;
}

.social {
  display: flex;
  justify-content: center;
}

.social a {
  color: black;
  margin: 20px;
  font-size: 3rem;
}

a:hover {
  font-size: 5rem;
  background-color: rgba( 255, 255, 255, 0.65 );
}
</style>
