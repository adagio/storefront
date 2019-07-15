<template>
  <div class="home-categories">
    <Category v-for="item in items"/> 
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
    items: Array
  },
  components: {
    Category
  }
};
</script>
