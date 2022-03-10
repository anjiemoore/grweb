<template>
  <div>
    <page-image-headers :headerImageText="headerImageText"></page-image-headers>
    <div class="difference-container">
      <h1>How We’re Different</h1>
      <div class="difference-list">
        <ul>
          <li>
            We offer the only 100% loyalty-based survey system, with all survey
            elements designed to help increase loyalty. These include:
            Likelihood to recommend, Likelihood to return, level of fun, and 3
            emotional loyalty questions; Net Promoter scoring of all attributes;
            all performance ratings broken down by Promoters, Passives and
            Detractors; and Detractor reasons.
          </li>
        </ul>
      </div>
      <div class="difference-subheaders">
        <h2>FOR THOSE WHO ARE TRULY SERIOUS ABOUT GUEST LOYALTY</h2>
        <br />
        <h2>WHY WE FOCUS ON LOYALTY</h2>
      </div>
      <div class="difference-loyalty">
        <ul>
          <li>
            While popular for decades, satisfaction surveys have failed to meet
            the needs and expectations of corporate America and other
            organizations. Unlike satisfaction, loyalty is proven to drive
            business performance.
          </li>
          <li>
            Created 18 years ago, the Likelihood to Recommend Net Promoter Score
            has become the universal measure of loyalty, the proven driver of
            higher visits, revenue, profits and market share. While satisfaction
            is necessary for loyalty, it is not sufficient, and adding only a
            Likelihood to Recommend question to a satisfaction survey does not
            make it a loyalty survey.
          </li>
          <li>
            Promoters build your business, while Detractors harm your business.
            Promoters visit, recommend write more positive reviews and spend
            more per visit than do Passives, and Passives do so more than
            Detractors. For these reasons, higher revenue and profits result
            from increasing the number and percentage of Promoters and
            decreasing the number and percentage of Detractors. The higher the
            Net Promoter Score, the greater the revenues and profits.
          </li>
          <li>
            Tracking these metrics by loyalty category is critical to
            calculating an ROI of your guest experience program.
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
  name: "Different",
  components: {
    PageImageHeaders,
    Footer,
  },
  props: {},
  data() {
    return {
      headerImageText: "Difference",
    };
  },
};
</script>

<style scoped>
* {
  margin: 0 auto;
}

h1 {
  font-size: 38px;
  font-family: "Impact";
  color: #358ddd;
  text-transform: uppercase;
  padding: 10px 0;
}
h2 {
  font-size: 16px;
  font-family: "Open Sans";
  color: rgb(102, 102, 102);
  font-weight: bold;
  line-height: 1.692;
  text-align: left;
}

ul,
li {
  font-size: 12px;
  font-family: "Open Sans";
  color: rgb(102, 102, 102);
  line-height: 1.833;
  text-align: left;
}
.difference-container {
  padding: 0 18px;
}
.difference-list {
  padding: 0 18px 20px;
}

.difference-loyalty {
  padding: 0 18px 60px;
}

.difference-subheaders {
  padding: 0 0 10px 0;
}
</style>
