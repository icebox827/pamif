<template>
  <section>
    <div class="image" :style="{ backgroundImage: `url( ${Image} )` }">
      <header>
        <h1>{{ msg }}</h1>
      </header>
      <div class="content">
        <div class="profile">
          <img src="../assets/dd.png" alt="Daniel Denis"/>
          <h5>Daniel Denis</h5>
          <h5>Coordonnateur de Terrain</h5>
        </div>
        <div class="pitch">
          <h2>Mot du Coordonnateur</h2>
          <p>
            Le Projet d'Appui pour une Meilleure Intégration des Femmes au sein de la Police Nationale d'Haïti (PAMIF-PNH),<br />
            a pour objectif de fournir un appui pédagogique supplémentaire aux jeunes filles désireuses de préparer le concours<br />
            d'admission à la PNH. Ce complément de formation s'ajoute au séances en présentiels qui sont dispenées dans les<br />
            départements géographiques prioritaires du projet, a savoir l'Ouest, l'Artibonite, le Nord et le Sud.
            <br />
            <br />
            Ce projet utilise un modèle hybride pour les séances de formation, une partie est dispensée en présentielle et l'autre<br />
            en ligne à travers notre plateforme de formation.
          </p>
        </div>
      </div>
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
  height: 87.5vh;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

.image h1 {
  text-align: center;
  padding-top: 15px;
}

.content {
  display: flex;
  justify-content: space-evenly;
  margin: 10px;
}

.profile img {
  border-radius: 20%;
  box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
}

.profile h5 {
  text-align: center;
  font-weight: 600;
  font-style: italic;
}

.pitch h2 {
  text-align: center;
  font-weight: 800;
}

.pitch p {
  font-weight: 700;
}
</style>
