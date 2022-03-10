<template>
  <div>
    <page-image-headers :headerImageText="headerImageText"></page-image-headers>
    <div class="about-container">
      <h1>WHO WE ARE</h1>
      <div class="about-list">
        <ul>
          <li>
            Guest Research, Inc. is a Denver-based, boutique research firm
            focusing exclusively on the leisure industry for the past 26 years.
          </li>
          <li>
            We provide a variety of quantitative research services, including
            customer satisfaction and loyalty measurement, employee opinion
            surveys, visitor studies and branding studies. Surveying is done
            online, with performance measured using Net Promoter Score scoring.
            All of our services are tailored to the needs of the client.
          </li>
          <li>
            Research data are available real-time to the client in a
            sophisticated, online Management Reporting System.
          </li>
        </ul>
      </div>
    </div>
    <Footer></Footer>
  </div>
</template>
<script>
import PageImageHeaders from "../components/PageImageHeaders.vue";
import Footer from "../components/Footer.vue";

export default {
  name: "About",
  components: {
    PageImageHeaders,
    Footer,
  },
  props: {},
  data() {
    return {
      headerImageText: "WHO WE ARE",
    };
  },
};
</script>

<style scoped>
.about-image-container {
  width: 100%;
  position: relative;
  text-align: center;
  color: white;
}

.about-image-text {
  width: 100%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 42px;
  font-family: "Impact";
  color: #fff;
  text-transform: uppercase;
  line-height: 0.223;
  text-shadow: 2px 2px 12px black;
}
* {
  margin: 0 auto;
}
h1 {
  font-size: 42px;
  font-family: "Impact";
  color: #358ddd;
  text-transform: uppercase;
  line-height: 0.223;
  padding: 20px 0;
}
ul,
li {
  font-size: 12px;
  font-family: "Open Sans";
  color: rgb(102, 102, 102);
  line-height: 1.833;
  text-align: left;
}

.about-list {
  padding: 10px 18px 40px;
}

img {
  /* display: block;
  max-width: 100%;
  max-height: 40%;
  width: auto;
  height: auto; */
  object-fit: cover;
  width: 100%;
  height: 150px;
}

.about-container {
  padding: 0 18px;
}
</style>
