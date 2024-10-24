<template>
  <div>
    <section class="container" id="productos">
      <h1 class="text-center">Contacto</h1>
      <RouterLink to="/">Volver al Inicio</RouterLink>
      <form class="col-md-6 my-5 m-auto">
        <h4 class="text-primary">Contáctanos</h4>
        <div class="mb-3">
          <label for="exampleFormControlInput1" class="form-label"
            >Correo</label
          >
          <input
            type="email"
            class="form-control"
            id="exampleFormControlInput1"
            placeholder="name@example.com"
          />
        </div>
        <div class="mb-3">
          <label for="exampleFormControlTextarea1" class="form-label"
            >Mensaje</label
          >
          <textarea
            class="form-control"
            id="exampleFormControlTextarea1"
            rows="3"
          ></textarea>
        </div>
        <button type="submit" class="btn btn-primary mb-5">Submit</button>
      </form>
    </section>
  </div>
</template>

<script>
import { RouterLink } from "vue-router";

export default {
  components: {
    RouterLink,
  },
};
</script>
