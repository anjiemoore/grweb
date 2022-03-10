<template>
  <div class="header-slideshow-container">
    <div class="header-slideshow-text">
      <h1>Our Mission</h1>
    </div>
    <swiper
      :navigation="false"
      :modules="modules"
      :loop="true"
      :autoplay="{
        delay: 3500,
        disableOnInteraction: true,
      }"
      class="mySwiper"
    >
      <swiper-slide>
        <img src="../assets/header-images/resort.jpg" />
      </swiper-slide>
      <swiper-slide>
        <img src="../assets/header-images/golf.jpg" />
      </swiper-slide>
      <swiper-slide>
        <img src="../assets/header-images/snow.jpg" />
      </swiper-slide>
      <swiper-slide>
        <img src="../assets/header-images/water.jpg" />
      </swiper-slide>
    </swiper>
  </div>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/navigation";

// import required modules
import { Autoplay, Navigation } from "swiper";

export default {
  name: "HeaderSlideshow",
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {};
  },
  setup() {
    return {
      modules: [Autoplay, Navigation],
    };
  },
};
</script>

<style scoped>
.swiper {
  height: 100%;
  width: 100%;
  /* border: 1px solid #000; */
}

.header-slideshow-container {
  position: relative;
}

.header-slideshow-text {
  width: 100%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 30px;
  font-family: "Impact";
  color: #fff;
  text-transform: uppercase;
  text-shadow: 2px 2px 12px black;
  z-index: 10;
}

img {
  width: 100%;
}
</style>
