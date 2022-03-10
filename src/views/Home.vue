<template>
  <div class="header-container">
    <div class="header-first-paragraph">
      <h1>RESEARCH <span class="blue">SERVICES</span></h1>
      <div class="header-paragraph-container">
        <p>
          Our research is uniquely designed with your company in mind and our
          state-of-the-art Management Reporting System allows for instant return
          on guest comments and ratings.
        </p>
      </div>
      <button class="header-demo-cta">REQUEST A DEMO</button>
    </div>
    <div class="header-who-we-are-section">
      <div class="header-who-we-are-text">
        <span class="black-text">Who We Are</span>
        <h2>
          OUR SERVICES ARE UNCONDITIONALLY<br /><span class="blue"
            >GUARANTEED</span
          >
        </h2>
        <router-link to="/about">Learn More</router-link>
      </div>
      <div class="header-who-we-are-image">
        <img src="../assets/revenue.png" />
      </div>
    </div>
    <!-- <div class="header-about-us-section">
      <h2>WHAT OUR CLIENTS <span class="blue">ARE SAYING</span></h2>
      <Quotes></Quotes>
    </div> -->
    <div class="header-possibilites-section">
      <h2>DISCOVER THE<span class="blue">possibilites</span></h2>
      <FeatureCard></FeatureCard>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
import FeatureCard from "../components/FeatureCard.vue";
import Footer from "../components/Footer.vue";
// import Quotes from "../components/Quotes.vue";

export default {
  name: "Home",
  components: {
    Footer,
    FeatureCard,
    // Quotes,
  },
};
</script>

<style scoped>
* {
  margin: 0 auto;
}
h1 {
  font-size: 44px;
  font-family: "Impact";
  color: rgb(167, 169, 172);
  text-transform: uppercase;
}

h2 {
  font-size: 44px;
  font-family: "Impact";
  color: rgb(167, 169, 172);
  text-transform: uppercase;
}

span {
  color: #358ddd;
  display: inline-block;
}

p {
  font-size: 14px;
  font-family: "Open Sans";
  color: rgb(102, 102, 102);
  line-height: 1.833;
  text-align: center;
}

.blue {
  display: inline-block;
}

.header-container {
  width: 100%;
  padding-bottom: 20px;
}
.header-first-paragraph {
  text-align: center;
}
.header-paragraph-container {
  padding: 15px 0;
}
.header-demo-cta {
  /* width: 70%; */
  font-size: 25px;
  font-family: "Impact";
  color: rgb(255, 255, 255);
  text-transform: uppercase;
  line-height: 1.5;
  text-align: center;
  border: none;
  border-radius: 10px;
  background-color: #358ddd;
  padding: 15px 15px;
  letter-spacing: 1.5px;
}
.header-who-we-are-section {
  padding: 60px 0;
  display: flex;
  justify-content: center;
  flex-direction: column;
}

.header-who-we-are-text {
  padding-bottom: 20px;
}

.header-who-we-are-image img {
  width: 100%;
  padding: 0 20px;
}

.black-text {
  font-size: 12px;
  font-family: "Open Sans";
  color: rgb(48, 48, 48);
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 2px;
}
a {
  font-size: 12px;
  font-family: "Open Sans";
  color: rgb(51, 104, 155);
  font-weight: bold;
  text-transform: uppercase;
  line-height: 1.2;
  text-align: center;
  text-decoration: none;
}
</style>
