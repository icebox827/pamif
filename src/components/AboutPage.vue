<template>
  <section>
    <div class="image" :style="{ backgroundImage: `url( ${Image} )` }">
      <h1>{{ msg }}</h1>
    </div>
  </section>
</template>

<script>
import Image from '@/assets/background2.png'

export default {
  data: () => ({
    Image
  }),
  name: 'ContactForm',
  props: {
    msg: String
  }
}
</script>

<style scoped>
.image {
  height: 88vh;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

.image h1 {
  text-align: center;
  padding-top: 15px;
}
</style>
