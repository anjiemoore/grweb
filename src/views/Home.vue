<template>
  <div class="header-container">
    <HeaderSlideshow></HeaderSlideshow>
    <div class="header-first-paragraph">
      <h2>RESEARCH <span class="blue">SERVICES</span></h2>
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
        <div class="who-we-are-text-wrapper">
          <span class="black-text">Who We Are</span>
          <h2>
            OUR SERVICES ARE UNCONDITIONALLY<br /><span class="blue"
              >GUARANTEED</span
            >
          </h2>
          <router-link to="/about">Learn More</router-link>
        </div>
      </div>
      <div class="header-who-we-are-image">
        <img src="../assets/revenue.png" />
      </div>
    </div>
    <div class="header-about-us-section">
      <h2>WHAT OUR CLIENTS <span class="blue">ARE SAYING</span></h2>
      <Quotes></Quotes>
    </div>
    <div class="header-possibilites-section">
      <h2>DISCOVER THE<span class="blue">&nbsp;possibilites</span></h2>
      <div class="header-card-container">
        <FeatureCard></FeatureCard>
      </div>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
import HeaderSlideshow from "@/components/HeaderSlideshow.vue";
import FeatureCard from "../components/FeatureCard.vue";
import Footer from "../components/Footer.vue";
import Quotes from "../components/Quotes.vue";

export default {
  name: "Home",
  components: {
    Footer,
    FeatureCard,
    HeaderSlideshow,
    Quotes,
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
  background-image: url("../assets/hp-bg.png") !important;
  background-repeat: no-repeat;
  background-position-x: right;
}
.header-first-paragraph {
  text-align: center;
}
.header-paragraph-container {
  padding: 15px 18px;
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

.header-card-container {
  padding: 30px 10px;
}
@media only screen and (min-width: 700px) {
  p {
    font-size: 14px;
  }
  .header-paragraph-container {
    width: 500px;
  }
  .header-who-we-are-section {
    justify-content: center;
    align-items: center;
    flex-direction: row-reverse;
  }
  .header-who-we-are-image img {
    padding: 0;
  }

  .header-who-we-are-text {
    min-width: 50%;
    text-align: left;
  }
  .who-we-are-text-wrapper {
    width: 500px;
    margin: 0;
  }
}
</style>
