<template>
  <Layout>
    <div class="hero hero--the-wedding">
      <video autoplay muted loop id="myVideo">
        <source src="../assets/videos/hero-video.mp4" type="video/mp4">Your browser does not support HTML5 video.
      </video>
    </div>
    <div class="content page-wrapper">
      <h1 class="title">The Wedding</h1>

      <div class="content-section">
        <h1>Ceremony & Reception</h1>

        <div class="labelled-content">
          <div class="label">When:</div>
          <div>
            <div>07.11.2020</div>
            <div>5:00PM - 11:00PM</div>
          </div>
        </div>

        <div class="labelled-content">
          <div class="label">Where:</div>
          <div>
            <div>
              Summit Chalet at Lutsen Mountains
              <br>455 Ski Hill Rd
              <br>Lutsen, MN 55612
            </div>
            <br>
            <iframe
              class="google-map"
              height="325"
              frameborder="0"
              src="https://www.google.com/maps/embed/v1/place?key=AIzaSyCiO2PXRZNnVBlW7hQxAnQUABJrGdP3b3c
    &q=Summit+Chalet+at+Lutsen+Mountains&zoom=11"
              allowfullscreen
            ></iframe>
          </div>
        </div>

        <div class="labelled-content">
          <div class="label">Agenda:</div>
          <div>
            <div>4:15PM</div>
            <div>Gondola will start taking guests up to Chalet for ceremony.</div>
            <br>
            <div>5:00PM</div>
            <div>Ceremony will begin.</div>
            <br>
            <div>5:30PM</div>
            <div>Cocktail hour directly following the ceremony.</div>
            <br>
            <div>6:00PM</div>
            <div>Dinner will be served.</div>
            <br>
            <div>7:00PM</div>
            <div>Shenanigans will ensue.</div>
            <br>
            <div>10:30PM</div>
            <div>Start heading to the gondola as the Chalet reception is complete.</div>
            <br>
            <div>10:30PM - 1:00AM</div>
            <div>After party at Papa Charlies with late night snacks to be served.</div>
          </div>
        </div>
      </div>

      <div class="content-section">
        <h1>Additional Information</h1>

        <div class="labelled-content">
          <div class="label">Dinner:</div>
          <div>Here’s my chance. You know what? It is beets. I’ve crashed into a beet truck. Is this my espresso machine? Wh-what is-h-how did you get my espresso machine?</div>
        </div>

        <div class="labelled-content">
          <div class="label">Bar:</div>
          <div>Beer and wine will be provided at no cost throughout the Chalet reception. Full cash bar for other drinks.</div>
        </div>

        <div class="labelled-content">
          <div class="label">Attire:</div>
          <div>
            Ladies, heels are highly discouraged! The Chalet’s decking is a grate for allowing snow to fall through in the winter.
            <br>
            <br>Please feel free to wear comfortable attire with potential for high temps in July.
          </div>
        </div>

        <div class="labelled-content">
          <div class="label">Gifts:</div>
          <div>Your presence is our present - no gifts please. If you feel inclined to give we have setup an account to donate to the National Parks.</div>
        </div>
      </div>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Wedding"
  }
};
</script>

<style lang="scss">
@import "../assets/scss/pages/_wedding.scss";
</style>