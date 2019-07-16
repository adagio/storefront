<template>
  <div class="home-categories">
    <Category v-for="item in category_items" :item="item"/> 
  </div>
</template>

<style lang="scss">
@import "../../styles/categories.scss";
</style>

<script>
import Category from "@/components/home/Category.vue";

export default {
  name: "Categories",
  props: {
    msg: String,
    category_items: Array
  },
  components: {
    Category
  }
};
</script>
