<template>
  <section>
    <div class="image" :style="{ backgroundImage: `url( ${Image} )` }">
        <h1>{{ msg }}</h1>
        <div class="card mb-3" style="max-width: 640px;">
          <div class="row g-0">
            <div class="col-md-4">
              <img src="../assets/LOGO.png" class="img-fluid rounded-start" alt="Logo">
              <h2>PAMIF-PNH</h2>
            </div>
            <div class="col-md-8">
              <div class="card-body">
                <form action="https://formspree.io/f/xjvjjvab" method="POST">
                  <fieldset>
                    <div class="mb-3">
                      <label for="exampleFormControlInput1" class="form-label">Adresse Email</label>
                      <input type="email" class="form-control" id="exampleFormControlInput1" name="email" placeholder="name@example.com">
                    </div>
                    <div class="mb-3">
                      <label for="exampleFormControlTextarea1" class="form-label">Contenu</label>
                      <textarea class="form-control" name="content" id="exampleFormControlTextarea1" rows="3"></textarea>
                    </div>
                    <div class="button">
                      <button type="submit" class="btn btn-primary">Envoyer</button>
                    </div>
                  </fieldset>
                </form>
              </div>
            </div>
          </div>
        </div>
    </div>
  </section>
</template>

<script>
import Image from '@/assets/background1.png'

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
  height: 92vh;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

h1 {
  padding-top: 15px;
  text-align: center;
}

.card {
  margin-left: auto;
  margin-right: auto;
  background-color: rgba(137, 152, 194, 0.65);
  border: 1px solid rgba(250, 235, 215, 0.473);
  border-radius: 10px;
  box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
  backdrop-filter: blur( 2.5px );
  -webkit-backdrop-filter: blur( 2.5px );
}

.card img {
  width: 20rem;
  margin-left: auto;
  margin-right: auto;
}

.card h2 {
  text-align: center;
}

.button {
  display: flex;
  justify-content: center;
}
</style>
