<template>
  <div class="home">
    <!-- <img alt="pamif logo" src="../assets/logo_pamif.png"> -->
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
