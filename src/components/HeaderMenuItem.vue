<template>
  <a class="header-menu-list-item" :href="item.slug">
    <div class="header-menu-list-item-img">
      <img v-bind:src="item.img_src" /> 
    </div>
    <div class="header-menu-list-item-text">
      {{ item.name }}
    </div>
  </a>
</template>

<script>
export default {
  name: "HeaderMenuItem",
  props: {
    item: Object
  }
};
</script>
