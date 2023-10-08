<template>
  <img
    class="mobile-menu__open-btn"
    src="../assets/images/icon-menu.svg"
    alt="Menu Button"
    v-on:click="toggleMenu"
  />
  <Transition name="fade">
    <div class="mobile-menu" id="mobile-menu" v-if="showMenu">
      <img
        src="../assets/images/icon-menu-close.svg"
        alt="Close Button"
        class="mobile-menu__close-btn"
        v-on:click="toggleMenu"
      />
      <ul class="mobile-menu__list">
        <li class="mobile-menu__list__item">Home</li>
        <li class="mobile-menu__list__item">New</li>
        <li class="mobile-menu__list__item">Popular</li>
        <li class="mobile-menu__list__item">Trending</li>
        <li class="mobile-menu__list__item">Categories</li>
      </ul>
    </div>
  </Transition>
</template>

<script>
export default {
  name: "MobileMenu",
  data() {
    return {
      showMenu: false,
    };
  },
  methods: {
    toggleMenu() {
      this.showMenu = !this.showMenu;
    },
  },
};
</script>
