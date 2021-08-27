<template>
 <section>
   <div class="hello">
      <div class="image" :style="{ backgroundImage: `url( ${Image} )` }">
        <h1>{{ msg }}</h1>
        <div class="content">
          <img alt="logo" src="../assets/LOGO.png">
          <div class="text">
            <h3>L'intégration des femmes dans les forces de l'ordre <br>est un atout majeur pour le renforcement de la sécurité
            </h3>
          </div>
        </div>
        <div class="social">
          <a href="#"><i class="fa fa-facebook-square" aria-hidden="true"></i></a>
          <a href="#">Twitter</a>
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
  height: 100vh;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

.image h1 {
  text-align: center;
  padding-top: 10px;
}

.content {
  width: 100%;
  display: flex;
  justify-content: space-between;
}

.content img {
  width: 25%;
  padding-left: 20px;
  margin-top: 5rem;
}

.text {
  display: flex;
  justify-content: flex-end;
  margin-top: 8rem;
}

.social {
  display: flex;
  justify-content: center;
}
</style>
