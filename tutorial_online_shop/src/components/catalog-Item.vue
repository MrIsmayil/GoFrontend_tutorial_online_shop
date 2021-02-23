<template>
  <div class="сatalog-item">
    <img
      class="product-img"
      :src="require('../assets/images/' + productData.image)"
      :alt="productData.image"
    />
    <p class="catalog-item-name">{{ productData.name }}</p>
    <p class="catalog-item-price">Price: {{ productData.price }} р.</p>
    <button class="catalog-item-add-button btn" @click="addToParent">
      Add to cart
    </button>
  </div>
</template>

<script>
export default {
  name: "сatalog-item",
  props: {
    productData: {
      type: Object,
      default() {
        return {};
      },
    },
  },
  data() {
    return {
      title: "Item 1",
    };
  },

  computed: {},
  methods: {
    addToParent() {
      this.$emit("sendingData", this.productData.category);
    },
  },
  watch: {},
  mounted() {
    console.log("Hello Catalog Item is aktive!");
  },
};
</script>

<style>
.сatalog-item {
  flex-basis: 25%;
  box-shadow: 0 0 8px 0 #e0e0e0;
  padding: 16px;
  margin-bottom: 16px;
  margin-top: 20px;
  margin-right: 2rem;
}

.product-img {
  width: 100%;
  height: 100%;
}
</style>
