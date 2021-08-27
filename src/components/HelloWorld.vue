<template>
 <section>
   <div class="hello">
    <div class="image" :style="{ backgroundImage: `url( ${Image} )` }">
      <img alt="pamif logo" src="../assets/logo_pamif.png">
      <h1>{{ msg }}</h1>
    </div>
  </div>
 </section>
 <section>
   <div class="content">
     <p></p>
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
</style>
