<template>
 <section>
   <div class="hello">
    <div class="image">
      <img alt="pamif logo" src="../assets/logo_pamif.png">
      <h1>{{ msg }}</h1>
    </div>
  </div>
 </section>
</template>

<script>
export default {
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
  background-image: url("https://unsplash.com/photos/jzonFmreWok?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
