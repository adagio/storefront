<template>
  <div class="home">
    <Header
      v-bind:menu_items="[
        {
          slug: 'aire-acondicionado',
          name: 'Aire acondicionado',
          img_src: './images/category_icons/aire-acondicionado.svg'
        },
        {
          slug: 'extractores',
          name: 'Extractores',
          img_src: './images/category_icons/coller-icon-header-nuevo.svg'
        },
        {
          slug: 'motores-electricos',
          name: 'Motores electricos',
          img_src: './images/category_icons/radiator_KMDt0CN.svg'
        },
        {
          slug: 'reductores',
          name: 'Reductores',
          img_src: './images/category_icons/reductores_UMgVrjr.svg'
        },
        {
          slug: 'controles-electricos',
          name: 'Controles Electricos',
          img_src: './images/category_icons/controles_WxmiqDn.svg'
        },
        {
          slug: 'tuberias-de-cobre',
          name: 'Tuberias de cobre',
          img_src: './images/category_icons/tuberias_Qzjdiv3.svg'
        },
        {
          slug: 'gas-refrigerante',
          name: 'Gas refrigerante',
          img_src: './images/category_icons/gas_e0t8HyM.svg'
        },
        {
          slug: 'fibra-de-vidrio',
          name: 'Fibra de vidrio',
          img_src: './images/category_icons/fibra_njEXbbL.svg'
        },
        {
          slug: 'poliuretano',
          name: 'Poliuretano',
          img_src: './images/category_icons/poliuterano_TPAW2sO.svg'
        }
      ]"
    />
    <Banner />
    <Categories
      v-bind:category_items="[
        {
          slug: 'extractores',
          img_src:
            'https://tienda.motorex.com.pe/media/category_name/3_RFjPdcL.jpg'
        },
        {
          slug: 'motores-electricos',
          img_src:
            'https://tienda.motorex.com.pe/media/category_name/1_AWCVD96.jpg'
        },
        {
          slug: 'tuberias-de-cobre',
          img_src:
            'https://tienda.motorex.com.pe/media/category_name/2_SfQkbDX.jpg'
        }
      ]"
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
</script>
