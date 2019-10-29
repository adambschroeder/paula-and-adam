<template>
  <header>
    <div class="header-message">
      <div class="page-wrapper">4284 days until we get hitched!</div>
    </div>
    <div class="main-header">
      <div>
        <nav class="page-wrapper">
          <g-link to="/">About Us</g-link>
          <g-link to="/wedding">The Wedding</g-link>
          <g-link to="/accommodations">Accommodations</g-link>
          <g-link to="/things-to-do">Things to Do</g-link>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style lang="scss">
@import "../styles/variables.scss";

header {
  .header-message {
    text-align: center;
    padding: 5px 0px;
  }

  .main-header {
    background-color: $primary-color;
    padding: 20px 0px;
  }

  nav {
    display: flex;
    justify-content: space-around;
  }

  a {
    color: $light-content-color;
    text-decoration: none;
  }

  a:hover {
    color: darken($light-content-color, 15%);
  }
}
</style>
