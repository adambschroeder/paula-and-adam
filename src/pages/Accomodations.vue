<template>
  <Layout>
    <div class="hero hero--the-wedding">
      <video autoplay muted loop id="myVideo">
        <source src="../assets/videos/hero-video.mp4" type="video/mp4" />Your browser does not support HTML5 video.
      </video>
    </div>
    <div class="content page-wrapper">
      <h1 class="title">Accomodations</h1>

      <div class="content-section">
        <h1>Eagle Ridge Resort</h1>
        <p>
          This is the resort the wedding is located and within walking distance of Gondola.
          <u>It does require two nights stay</u> but within the wedding block there is a small discount or a free 3rd night.
          Also, condos available to accomodate larger groups.
        </p>
        <p>To book, follow these steps:</p>
        <ol>
          <li>
            Call up
            <a href="tel:1-218-406-1350">218.406.1350</a>
          </li>
          <li>Mention the booking is part of the 'July 11th Schroeder wedding'</li>
          <li>Confirm a 10% discount on a 2-night reservation or a 3rd night free</li>
        </ol>
        <iframe
          class="google-map"
          height="325"
          frameborder="0"
          src="https://www.google.com/maps/embed/v1/place?key=AIzaSyCiO2PXRZNnVBlW7hQxAnQUABJrGdP3b3c
    &q=Eagle+Ridge+Resort+Lutsen&zoom=11"
          allowfullscreen
        ></iframe>
      </div>

      <div class="content-section">
        <h1>Other Accomodations</h1>
        <p>
          There are some other options, potentially cheaper, though they would require driving and if there is drinking in your future
          we would highly recommend y'all not to drive - please. Other options may also not have the two-night requiremt though a rarity.
        </p>

        <ul>
          <li>
            <a href="//caribouhighlands.com/" target="_blank">Caribou Highlands</a>: 2min drive / 11min walk from the gondola.
          </li>
          <li>
            <a href="//www.lutsenresort.com/" target="_blank">Lutsen Resort</a>: 5min drive down the hill from the gondola - on the lake.
          </li>
          <li>
            <a href="//www.airbnb.com">Airbnb</a>: variable locations but could accomodate a larger group.
          </li>
        </ul>
      </div>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Accomodations"
  }
};
</script>
