<template>
  <swiper :navigation="true" :modules="modules" :loop="true" class="mySwiper">
    <swiper-slide>
      <div class="card"><p>general kenobi</p></div>
    </swiper-slide>
    <swiper-slide>Slide 2</swiper-slide>
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

export default {
  name: "FeatureCard",
  components: {
    Swiper,
    SwiperSlide,
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
