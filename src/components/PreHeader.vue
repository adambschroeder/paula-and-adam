<template>
  <div class="pre-header">
    <div class="page-wrapper">{{daysToWedding}} days until we get hitched!</div>
  </div>
</template>

<script>
export default {
  name: "PreHeader",
  data() {
    return {
      daysToWedding: 0
    };
  },
  created() {
    var oneDay = 24 * 60 * 60 * 1000; // hours*minutes*seconds*milliseconds
    var today = new Date(); // 29th of Feb at noon your timezone
    var weddingDate = new Date(2020, 6, 11, 5, 0, 0, 0); // 2st of March at noon

    this.daysToWedding = Math.round(
      Math.abs((today.getTime() - weddingDate.getTime()) / oneDay)
    );
  }
};
</script>

<style lang="scss">
@import "../assets/scss/components/preHeader";
</style>
