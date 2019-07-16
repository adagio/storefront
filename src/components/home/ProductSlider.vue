<template>
  <div class="product-slider">
    <div class="product-slider-title">
      Encuentra tu producto ideal
    </div>
    <div class="product-slider-content">
      <div class="product-slider-list">
        <Product v-for="item in items"/>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@import "../../styles/products.scss";
</style>

<script>
import Product from "@/components/home/Product.vue";

export default {
  name: "ProductSlider",
  props: {
    items: Array
  },
  components: {
    Product
  }
};
</script>
