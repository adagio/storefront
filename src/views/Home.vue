<template>
  <div class="home">
    <Header v-bind:menu_items="[1, 2, 3, 4, 5, 6, 7, 8, 9]" />
    <Banner />
    <Categories
      v-bind:items="[{ name: Extractores }, { name: Aire }, { name: Agua }]"
    />
    <div class="container">
      <ProductSlider v-bind:items="[1, 2, 3, 4]" />
    </div>
    <div class="container">
      <PromotionalGrid />
    </div>
    <div class="container">
      <BrandSlider />
    </div>
    <div class="container">
      <Social />
    </div>
    <div class="container">
      <Newsletter />
    </div>
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from "@/components/Header.vue";
import Banner from "@/components/home/Banner.vue";
import Categories from "@/components/home/Categories.vue";
import ProductSlider from "@/components/home/ProductSlider.vue";
import PromotionalGrid from "@/components/home/PromotionalGrid.vue";
import BrandSlider from "@/components/home/BrandSlider.vue";
import Social from "@/components/home/Social.vue";
import Newsletter from "@/components/home/Newsletter.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "home",
  components: {
    Header,
    Banner,
    Categories,
    ProductSlider,
    PromotionalGrid,
    BrandSlider,
    Social,
    Newsletter,
    Footer
  }
};

/*
 {'name': 'Aire Acondicionado'},{name:
    'Extractores'},{name: 'Motores Electricos'},{name:'Reductores'},{name:'Controles
    Electricos'}, {name: 'Tuberias de Cobre'},{name: 'Gas refriferante'},
    {name:'Fibra de Vidrio'}, {name: 'Poliuretano'}

*/
</script>
