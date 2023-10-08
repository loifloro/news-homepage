<template>
  <header class="menu">
    <img src="../assets/images/logo.svg" alt="Logo" class="menu__logo" />
    <nav class="menu__nav">
      <ul class="menu__list">
        <li class="menu__list__item">Home</li>
        <li class="menu__list__item">New</li>
        <li class="menu__list__item">Popular</li>
        <li class="menu__list__item">Trending</li>
        <li class="menu__list__item">Categories</li>
      </ul>
    </nav>

    <MobileMenu />
  </header>
</template>

<script>
import MobileMenu from "./MobileMenu.vue";

export default {
  name: "Header",
  components: {
    MobileMenu,
  },
};
</script>
