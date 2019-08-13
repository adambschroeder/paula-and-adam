<template>
  <Layout>
    <div class="hero hero--about-us">
      <div class="circle-arrow">
        <span class="bounceAlpha arrow primera next"></span>
        <span class="bounceAlpha arrow segunda next"></span>
      </div>
    </div>

    <div class="content content--with-hero page-wrapper">
      <h1 class="title">About Us</h1>

      <div class="content-section">
        <h1>How We Met</h1>
        <div class="sub-header">12.11.2011</div>
        <p>You really think you can fly that thing? Life finds a way. What do they got in there? King Kong? God help us, we’re in the hands of engineers. Yeah, but your scientists were so preoccupied with whether or not they could, they didn’t stop to think if they should.</p>

        <h1>The Proposal</h1>
        <div class="sub-header">08.09.2020</div>
        <p>They’re using our own satellites against us. And the clock is ticking. This thing comes fully loaded. AM/FM radio, reclining bucket seats, and… power windows. Remind me to thank John for a lovely weekend. Just my luck, no ice. Did he just throw my cat out of the window?</p>

        <h1>About Us</h1>
        <p>From Paula:</p>
        <p>Just my luck, no ice. Yeah, but your scientists were so preoccupied with whether or not they could, they didn’t stop to think if they should. Hey, you know how I’m, like, always trying to save the planet? Here’s my chance. What do they got in there? King Kong?</p>

        <p>From Adam:</p>
        <p>Yeah, but John, if The Pirates of the Caribbean breaks down, the pirates don’t eat the tourists. They’re using our own satellites against us. And the clock is ticking. Hey, you know how I’m, like, always trying to save the planet? Here’s my chance. They’re using our own satellites against us. And the clock is ticking.</p>
      </div>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "About Us"
  },
  methods: {
    handleScroll(event) {
      document
        .querySelector(".circle-arrow")
        .classList.add("animated", "fadeOut");
    }
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },
  destroyed() {
    window.removeEventListener("scroll", this.handleScroll);
  }
};
</script>

<style lang="scss">
@import "../assets/scss/pages/_index.scss";
</style>
