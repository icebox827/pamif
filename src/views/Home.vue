<template>
  <div class="home">
    <HelloWorld msg="Bienvenue à PAMIF-PNH"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style>
.home {
  text-align: center;
  color: rgb(78, 92, 116);
}
</style>
