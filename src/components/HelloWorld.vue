<template>
 <section>
   <div class="hello">
    <h1>{{ msg }}</h1>
    <div :style="image" class="image"></div>
  </div>
 </section>
</template>

<script>
export default {
  data () {
    return {
      image: { backgroundImage: 'url(https://unsplash.com/photos/jzonFmreWok?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink)' }
    }
  },
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.image {
  width: 100%;
  height: 100vh;
}
</style>
