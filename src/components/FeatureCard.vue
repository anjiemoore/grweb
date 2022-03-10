<template>
  <swiper :navigation="true" :modules="modules" :loop="true" class="mySwiper">
    <swiper-slide>
      <card
        :cardImage="cardImage1"
        :cardTitle="cardTitle1"
        :cardBody="cardBody1"
      ></card>
    </swiper-slide>
    <swiper-slide>
      <card :cardTitle="cardTitle2" :cardBody="cardBody2"></card>
    </swiper-slide>
    <swiper-slide>Slide 3</swiper-slide>
    <swiper-slide>Slide 4</swiper-slide>
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
      cardImage1: "https://via.placeholder.com/150",
      cardTitle1: "hello there",
      cardBody1: "general kenobi",
      cardTitle2: "is this the krusty krab?",
      cardBody2: "gi",
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
  height: 300px;
  width: 100%;
  /* border: 1px solid #000; */
}

.card {
  border: 1px solid #000;
  width: 50%;
  margin: 0 auto;
}
</style>
