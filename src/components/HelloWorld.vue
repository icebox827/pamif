<template>
 <section>
   <div class="hello">
      <div class="image" :style="{ backgroundImage: `url( ${Image} )` }">
        <h1>{{ msg }}</h1>
        <div class="content d-flex mt-2 justify-between">
          <img alt="logo" src="../assets/LOGO.png">
          <h3>Une programme de formation accélérée</h3>
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
  width: 80%;
  border: 1px solid gray;
}

.content img {
  width: 25%;
  padding-left: 20px;
}

.content h3 {
  width: 50%;
}
</style>
