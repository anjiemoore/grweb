<template>
  <swiper
    :navigation="true"
    :modules="modules"
    :loop="true"
    :breakpoints="swiperOptions.breakpoints"
    class="mySwiper"
  >
    <swiper-slide>
      <card
        :cardImage="cardImage1"
        :cardTitle="cardTitle1"
        :cardBody="cardBody1"
      ></card>
    </swiper-slide>
    <swiper-slide>
      <card
        :cardImage="cardImage2"
        :cardTitle="cardTitle2"
        :cardBody="cardBody2"
      ></card>
    </swiper-slide>
    <swiper-slide
      ><card
        :cardImage="cardImage3"
        :cardTitle="cardTitle3"
        :cardBody="cardBody3"
      ></card
    ></swiper-slide>
    <swiper-slide
      ><card
        :cardImage="cardImage4"
        :cardTitle="cardTitle4"
        :cardBody="cardBody4"
      ></card
    ></swiper-slide>
  </swiper>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/navigation";

// import required modules
import { Navigation } from "swiper";
import Card from "./Card.vue";

export default {
  name: "FeatureCard",
  components: {
    Swiper,
    SwiperSlide,
    Card,
  },
  data() {
    return {
      cardImage1: require(`@/assets/svgs/feedback2.svg`),
      cardTitle1: `<span style="color: #34C6A6;">Realtime</span><br>Feedback`,
      cardBody1:
        "Real-time feedback supports continuous improvement throughout your organization",
      cardImage2: require(`@/assets/svgs/loyalty.svg`),
      cardTitle2: `<span style="color: #34C6A6;">Higher Satisfaction</span> and&nbsp;Loyalty`,
      cardBody2:
        "Continuous feedback and product enhancements create higher satisfaction and loyalty",
      cardImage3: require(`@/assets/svgs/repeat2.svg`),
      cardTitle3: `<span style="color: #34C6A6;">Higher</span> Repeat and&nbsp;Referrals`,
      cardBody3:
        "Higher satisfaction and loyalty produce higher repeat and referral business",
      cardImage4: require(`@/assets/svgs/profits2.svg`),
      cardTitle4: `<span style="color:#34C6A6;">Higher</span> Revenues and&nbsp;Profits`,
      cardBody4:
        "Higher repeat business and referrals are the keys to higher revenues and profits",
      swiperOptions: {
        breakpoints: {
          700: {
            slidesPerView: 4,
          },
        },
      },
    };
  },
  setup() {
    return {
      modules: [Navigation],
    };
  },
};
</script>

<style scoped>
.swiper {
  height: 280px;
  width: 100%;
  /* border: 1px solid #000; */
}

.card {
  border: 1px solid #000;
  width: 50%;
  margin: 0 auto;
}

/deep/ .swiper-button-prev {
  left: 0 !important;
  top: 46% !important;
  background-color: #fff !important;
  color: #4fc0a7 !important;
  fill: #4fc0a7 !important;
  stroke: #4fc0a7 !important;
}
/deep/ .swiper-button-next {
  right: 0 !important;
  top: 46% !important;
  background-color: #fff !important;
  color: #4fc0a7 !important;
  fill: #4fc0a7 !important;
  stroke: #4fc0a7 !important;
}
@media only screen and (min-width: 700px) {
  /deep/ .swiper-button-prev {
    display: none;
  }
  /deep/ .swiper-button-next {
    display: none;
  }
}
</style>
