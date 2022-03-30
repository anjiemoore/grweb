<template>
  <div>
    <page-image-headers :headerImageText="headerImageText"></page-image-headers>
    <div class="nps-container">
      <div class="nps-inner">
        <h1>OUR NET PROMOTER SYSTEM</h1>
        <div class="nps-list">
          <ul>
            <li>
              Surveys may be of any length to fit most any budget; our shorter
              surveys typically have 2-40 questions.
            </li>
            <li>
              Guest feedback is captured online and real-time via post-departure
              surveying.
            </li>
            <li>
              Captured feedback resides in a custom-designed, high functionality
              online Management Reporting System (“MRS”) that now includes a
              Correlation Calculator to quantify what’s important to your
              guests.
            </li>
            <li>
              Surveys include quantitative ratings, open-end comments and
              marketing/profile questions.
            </li>
            <li>
              All feedback can be easily segmented by guest segment, demographic
              variables and other marketing variables.
            </li>
            <li>
              Benchmarking to similar-quality competitors may be available.
            </li>
            <li>
              Complimentary consultative support, Industry Best Practices and
              personalized service are provided by our Account Managers to help
              drive higher revenues.
            </li>
            <li>All services are unconditionally guaranteed.</li>
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
import SideButtons from "../components/SideButtons.vue";
import Footer from "../components/Footer.vue";
export default {
  name: "NpsSystem",
  components: {
    PageImageHeaders,
    SideButtons,
    Footer,
  },
  props: {},
  data() {
    return {
      headerImageText: "NPS System",
    };
  },
};
</script>

<style scoped>
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
.nps-container {
  padding: 0 18px;
  display: flex;
}
.nps-list {
  padding: 0 18px 20px;
}

.nps-loyalty {
  padding: 0 18px 60px;
}

.nps-subheaders {
  padding: 0 0 10px 0;
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
  .nps-container {
    width: 60%;
    flex-direction: row;
    align-items: baseline;
  }
  .nps-inner {
    padding-right: 20px;
    width: 64%;
  }
}
</style>
