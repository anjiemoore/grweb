<template>
  <div>
    <page-image-headers :headerImageText="headerImageText"></page-image-headers>
    <div class="about-container">
      <div class="about-inner">
        <h1>WHO WE ARE</h1>
        <div class="about-list">
          <ul>
            <li>
              Guest Research, Inc. is a Denver-based, boutique research firm
              focusing exclusively on the leisure industry for the past 26
              years.
            </li>
            <li>
              We provide a variety of quantitative research services, including
              customer satisfaction and loyalty measurement, employee opinion
              surveys, visitor studies and branding studies. Surveying is done
              online, with performance measured using Net Promoter Score
              scoring. All of our services are tailored to the needs of the
              client.
            </li>
            <li>
              Research data are available real-time to the client in a
              sophisticated, online Management Reporting System.
            </li>
          </ul>
        </div>
      </div>
      <side-buttons></side-buttons>
    </div>
    <Footer></Footer>
  </div>
</template>
<script>
import PageImageHeaders from "../components/PageImageHeaders.vue";
import Footer from "../components/Footer.vue";
import SideButtons from "@/components/SideButtons.vue";

export default {
  name: "About",
  components: {
    PageImageHeaders,
    SideButtons,
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
.about-container {
  padding: 0 18px;
  display: flex;
}

* {
  margin: 0 auto;
}
h1 {
  font-size: 42px;
  font-family: "Impact";
  color: #358ddd;
  text-transform: uppercase;
  padding-top: 20px;
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

.about-container {
  padding: 0 18px;
}
@media only screen and (min-width: 700px) {
  h1,
  h2 {
    text-align: left;
  }
  ul,
  li {
    font-size: 14px;
  }
  .about-container {
    width: 60%;
    flex-direction: row;
    align-items: baseline;
  }
  .about-inner {
    padding-right: 20px;
    width: 64%;
  }
}
</style>
