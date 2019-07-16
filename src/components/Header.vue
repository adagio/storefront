<template>
  <header class="header">
    <div class="header-message">
      <div class="container">
        <div class="header-message-text">
          APROVECHA EL 50% EN AIRES ACONDICIONADOS
        </div>
      </div>
    </div>
    <div class="container">
      <div class="header-top">
        <div class="header-top-left">
          <div class="header-logo">
            <a href="/">
              <img
                src="https://res.cloudinary.com/jtantadiaz/image/upload/v1548195881/motorex/motorex-logo-v.png"
              />
            </a>
          </div>
        </div>
        <div class="header-top-middle">
          <form id="form_search" method="GET" action="/results/">
            <div class="header-top-middle-search">
              <input
                type="text"
                placeholder="Encuentra tu producto"
                id="search_value"
                name="search_value"
                autocomplete="off"
                pattern=".{3,}"
                title="3 caracteres como mínimo"
              />
              <span id="search" class="icon-search"></span>
            </div>
          </form>
        </div>
        <div class="header-top-right">
          <a class="header-icon-link" href="/seguimiento">
            <span class="icon-shipped"></span>
            <div class="header-icon-link-text">
              SIGUE TU PEDIDO
            </div>
          </a>
          <div class="header-icon-link">
            <span class="icon-account"></span>
            <div class="header-icon-link-text">
              MI CUENTA
            </div>
          </div>
          <div class="header-icon-link cart">
            <span class="icon-cart">
              <div class="number">
                0
              </div>
            </span>
            <div class="header-icon-link-text">
              US$ 0.00
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="header-box-shadow"></div>
    <div class="container">
      <HeaderMenu v-bind:items="menu_items" />
    </div>
    <HeaderMobile />
  </header>
</template>

<style>
@import "../styles/_variables.scss";
@import "../styles/global.scss";
@import "../styles/header.scss";
</style>

<script>
import HeaderMenu from "@/components/HeaderMenu.vue";
import HeaderMobile from "@/components/HeaderMobile.vue";

export default {
  name: "Header",
  props: {
    msg: String,
    menu_items: Array
  },
  components: {
    HeaderMenu,
    HeaderMobile
  }
};
</script>
