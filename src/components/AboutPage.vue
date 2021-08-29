<template>
  <section>
    <div class="image" :style="{ backgroundImage: `url( ${Image} )` }">
      <h1>{{ msg }}</h1>
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
