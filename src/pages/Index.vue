<template>
  <Layout>
    <div class="hero hero--about-us">
      <div class="arrows-container">
        <span class="bounceAlpha arrow primera next"></span>
        <span class="bounceAlpha arrow segunda next"></span>
      </div>
    </div>

    <div class="content content--with-hero page-wrapper">
      <h1 class="title">About Us</h1>

      <div class="content-section content-section--flush">
        <video
          style="width: 100%; display: block;"
          src="../assets/videos/proposal-video.mp4"
          controls
        ></video>
      </div>
      <div class="content-section">
        <h1>Our Story</h1>
        <p>
          It was winter break in 2012, Adam and
          Paula were both living in the same (crappy)
          apartment complex at Minnesota State University,
          Mankato. Paula and her roommate Jaime were
          bored one night and invited their friend Garret
          over, who showed up with Adam. Right away, Paula
          felt like she knew Adam her whole life, and Adam thought
          Paula was cute in her camouflage sweatpants.
        </p>
        <p>
          ...after winter break we ended up in the same class and the
          good times rolled. We even spent some time working
          together at Menards. Soon after, we began our relationship
          which has always been based on a strong friendship,
          laughter, and supporting one another. We make a great team. Together
          we have developed a strong love for travel, good beer,
          and making the most out of this crazy, wonderful life!
        </p>
      </div>

      <div class="content-section">
        <ClientOnly>
          <carousel :centerMode="true" :perPage="1" :paginationSize="7">
            <slide>
              <g-image src="../assets/images/slideshow2.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow3.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow5.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow6.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow15.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow4.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow8.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow10.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow11.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow1.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow13.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow7.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow14.jpg" />
            </slide>
            <slide>
              <g-image src="../assets/images/slideshow9.jpg" />
            </slide>
          </carousel>
        </ClientOnly>
      </div>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "About Us"
  },
  components: {
    Carousel: () =>
      import("vue-carousel")
        .then(m => m.Carousel)
        .catch(),
    Slide: () =>
      import("vue-carousel")
        .then(m => m.Slide)
        .catch()
  },
  data() {
    return {
      flickityOptions: JSON.stringify({
        pageDots: false,
        wrapAround: true
      })
    };
  },
  methods: {
    handleScroll(event) {
      document
        .querySelector(".arrows-container")
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
