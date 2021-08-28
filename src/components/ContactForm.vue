<template>
  <section>
    <h1>{{ msg }}</h1>
    <div class="form">
      <form action="">
        <div class="mb-3">
          <label for="exampleFormControlInput1" class="form-label">Email address</label>
          <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="name@example.com">
        </div>
        <div class="mb-3">
          <label for="exampleFormControlTextarea1" class="form-label">Example textarea</label>
          <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
        </div>
        <button type="submit" class="btn btn-primary">Submit</button>
      </form>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ContactForm',
  props: {
    msg: String
  }
}
</script>

<style scoped>
  h1 {
    margin-top: 15px;
    text-align: center;
  }
</style>
