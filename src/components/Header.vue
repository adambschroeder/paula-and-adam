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
          <g-link to="/accomodations">Accomodations</g-link>
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

    <div
      class="nav-mobile-menu page-wrapper animated"
      v-bind:class="{ 'is-active slideInRight': isMenuOpen }"
    >
      <g-link to="/">Our Story</g-link>
      <g-link to="/wedding">Wedding</g-link>
      <g-link to="/accomodations">Accomodations</g-link>
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
    animate: function(selector, animationName, callback) {
      const node = document.querySelector(selector);
      node.classList.add("animated", animationName);

      function handleAnimationEnd() {
        node.classList.remove("animated", animationName);
        node.removeEventListener("animationend", handleAnimationEnd);

        if (typeof callback === "function") callback();
      }

      node.addEventListener("animationend", handleAnimationEnd);
    },
    displayMenu: function(event) {
      var self = this;
      self.isBurgerOpen = !self.isBurgerOpen;

      if (self.isMenuOpen) {
        self.animate(".nav-mobile-menu", "slideOutRight", function() {
          self.isMenuOpen = false;
        });
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
