<template>
  <div class="header-menu" >
    <div class="header-menu-ctn">
      <ul class="header-menu-list">
        <HeaderMenuItem v-for="item in items"/> 
      </ul>
    </div>
  </div> 
</template>

<style lang="scss">
@import "../styles/header_menu.scss";
</style>

<script>
import HeaderMenuItem from "@/components/HeaderMenuItem.vue";

export default {
  name: "HeaderMenu",
  props: {
    items: Array
  },
  components: {
    HeaderMenuItem
  }
};
</script>
