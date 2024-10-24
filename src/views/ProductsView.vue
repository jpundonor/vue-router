<template>
  <div>
    <section class="container" id="productos">
      <h1 class="text-center">Productos</h1>
      <RouterLink to="/">Volver al Inicio</RouterLink>
      <div class="row my-5">
        <div class="col-md-4 my-4" v-for="product in products" :key="product.id">
          <!-- Component Product with props -->
          <Product
            :name="product.name"
            :description="product.description"
            :price="product.price"
            :quantity="product.quantity"
          />
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import { RouterLink } from "vue-router";
import Product from "../components/Product.vue";

export default {
  components: {
    RouterLink,
    Product,
  },
  data() {
    return {
      products: [
        {
          id: 1,
          name: "Colaciones",
          description:
            "Some quick example text to build on the card title and make up the bulk of the card's content.",
          price: 500,
          quantity: "Por unidad",
        },
        {
          id: 2,
          name: "Bebidas",
          description:
            "Some quick example text to build on the card title and make up the bulk of the card's content.",
          price: 500,
          quantity: "Por unidad",
        },
        {
          id: 3,
          name: "Desayunos",
          description:
            "Some quick example text to build on the card title and make up the bulk of the card's content.",
          price: 1000,
          quantity: "Para 2 personas",
        },
        {
          id: 4,
          name: "Empanadas",
          description:
            "Some quick example text to build on the card title and make up the bulk of the card's content.",
          price: 2000,
          quantity: "Por unidad",
        },
        {
          id: 5,
          name: "Dulces",
          description:
            "Some quick example text to build on the card title and make up the bulk of the card's content.",
          price: 1500,
          quantity: "Por unidad",
        },
        {
          id: 6,
          name: "Verduras",
          description:
            "Some quick example text to build on the card title and make up the bulk of the card's content.",
          price: 2500,
          quantity: "Por unidad",
        },
      ],
    };
  },
};
</script>
