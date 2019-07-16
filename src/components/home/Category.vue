<template>
  <a :href="item.slug" class="home-categories-item">
    <img :src="item.img_src" alt="" />
  </a>
</template>

<script>
export default {
  name: "Category",
  props: {
    item: Object
  }
};
</script>
