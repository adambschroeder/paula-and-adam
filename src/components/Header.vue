<template>
  <header>
    <nav>
      <div class="nav-items page-wrapper">
        <div class="nav-logo">
          <g-link to="/">Paula & Adam</g-link>
        </div>
        <div class="nav-links">
          <g-link to="/">About Us</g-link>
          <g-link to="/wedding">Wedding</g-link>
          <g-link to="/accommodations">Accommodations</g-link>
          <g-link to="/north-shore">North Shore</g-link>
        </div>

        <div class="nav-burger">
          <button
            class="hamburger hamburger--collapse"
            type="button"
            v-on:click="displayMenu"
            v-bind:class="{ 'is-active': isBurgerOpen }"
          >
            <span class="hamburger-box">
              <span class="hamburger-inner"></span>
            </span>
          </button>
        </div>
      </div>
    </nav>

    <div class="nav-mobile-menu page-wrapper" v-bind:class="{ 'is-active': isMenuOpen }">
      <g-link to="/">Our Story</g-link>
      <g-link to="/wedding">Wedding</g-link>
      <g-link to="/accommodations">Accommodations</g-link>
      <g-link to="/north-shore">North Shore</g-link>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data: function() {
    return {
      isBurgerOpen: false,
      isMenuOpen: false
    };
  },
  methods: {
    displayMenu: function(event) {
      var self = this;
      self.isBurgerOpen = !self.isBurgerOpen;

      if (self.isMenuOpen) {
        self.isMenuOpen = false;
      } else {
        self.isMenuOpen = true;
      }
    }
  }
};
</script>

<style lang="scss">
@import "../assets/scss/components/header";
</style>
