<template>
  <header>
    <!-- <div class="main-header">
      <div class="main-header-inner page-wrapper">
    <div class="header-nav">-->
    <nav class="page-wrapper">
      <g-link to="/">About Us</g-link>
      <g-link to="/wedding">The Wedding</g-link>
      <img class="header-logo" src="../assets/svg/header-logo.svg" alt="Paula & Adam 7.11.2020">
      <g-link to="/accomodations">Accomodations</g-link>
      <g-link to="/things-to-do">Things to Do</g-link>
    </nav>
    <!-- </div>
      </div>
    </div>-->
  </header>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style lang="scss">
@import "../assets/scss/components/header";
</style>
