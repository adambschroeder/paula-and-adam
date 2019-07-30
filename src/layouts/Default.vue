<template>
  <div class="layout">
    <PreHeader/>
    <Header/>
    <slot/>
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<script>
import PreHeader from "~/components/PreHeader.vue";
import Header from "~/components/Header.vue";

export default {
  components: {
    PreHeader,
    Header
  }
};
</script>

<style lang="scss">
@import "../assets/scss/main.scss";
@import "../assets/scss/layouts/_default.scss";
</style>


