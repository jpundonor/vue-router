<template>
  <div class="card">
    <img
      src="../assets/img/colaciones.jpg"
      class="card-img-top"
      alt="colaciones"
    />
    <div class="card-body">
      <h5 class="card-title fw-bold">{{ name }}</h5>
      <p class="card-text">
        {{ description }}
      </p>
    </div>
    <ul class="list-group list-group-flush">
      <li class="list-group-item">Precio: ${{ price }}</li>
      <li class="list-group-item">Cantidad: {{ quantity }}</li>
    </ul>
    <div class="card-body">
      <a href="#" class="card-link">Ver más</a>
      <a href="#" class="card-link">Comprar</a>
    </div>
  </div>
</template>
<script>
export default {
  name: "Product",
  props: ["name", "description", "price", "quantity"],
};
</script>
<style scoped></style>
