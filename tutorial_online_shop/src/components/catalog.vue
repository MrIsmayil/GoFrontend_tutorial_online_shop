<template>
  <section class="catalog">
    <h1>{{ title }}</h1>
    <div class="productCard">
      <catalog-item
        v-for="product in products"
        :key="product.article"
        :productData="product"
        @sendingData="dataFromChild"
      />
    </div>
  </section>
</template>

<script>
import CatalogItem from "./catalog-Item";

export default {
  name: "catalog",
  components: {
    CatalogItem,
  },
  props: {},
  data() {
    return {
      title: "Catalog!",
      products: [
        {
          image: "1.jpg",
          name: "T-shirt 1",
          price: 100.05,
          article: "T1",
          available: true,
          category: "Мужские",
        },
        {
          image: "2.jpg",
          name: "T-shirt 2",
          price: 150.12,
          article: "T2",
          available: true,
          category: "Женские",
        },
        {
          image: "3.jpg",
          name: "T-shirt 3",
          price: 200.15,
          article: "T3",
          available: false,
          category: "Женские",
        },
        {
          image: "4.jpg",
          name: "T-shirt 4",
          price: 250.23,
          article: "T4",
          available: true,
          category: "Мужские",
        },
        {
          image: "5.jpg",
          name: "T-shirt 5",
          price: 300.32,
          article: "T5",
          available: false,
          category: "Женские",
        },
        {
          image: "6.jpg",
          name: "T-shirt 6",
          price: 350.38,
          article: "T6",
          available: true,
          category: "Женские",
        },
      ],
    };
  },

  computed: {},
  methods: {
    dataFromChild(data) {
      console.log(data);
    },
  },
  watch: {},
  mounted() {
    console.log("Hello Catalog is aktive!");
  },
};
</script>

<style>
.catalog {
  flex-direction: column;
}

.productCard {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  margin-bottom: 20px;
}

h1 {
  justify-content: center;
}
</style>
