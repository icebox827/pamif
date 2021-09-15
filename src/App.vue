<template>
  <div id="nav">
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
      <div class="container-fluid">
         <a class="navbar-brand" href="#">
            <!-- <img alt="pamif logo" src="../assets/logo_pamif.png"> -->
          </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <router-link class="nav-link active" aria-current="page" to="/">Acceuil</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/about">A propos</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/contact">Contact</router-link>
            </li>
          </ul>
          <div class="d-flex">
            <a href="https://learn.cowater-pamifpnh.com" target="_blank">Plateforme Éducative</a>
          </div>
        </div>
      </div>
    </nav>
  </div>
  <router-view/>
  <Footer />
</template>

<script>
import Footer from '@/components/Footer.vue'

export default {
  components: {
    Footer
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#nav {
  background-color: rgb(69, 86, 236);
}

#nav a {
  font-weight: bold;
  color: white;
}

#nav a.router-link-exact-active {
  color: #f33f1f;
}

nav a {
  text-decoration: none;
}

a:hover {
  background-color: rgb(124, 175, 252);
  font-size: larger;
}
</style>
