<template>
  <div>
    <div class="about-image-container">
      <img src="../assets/stock-images/pexels-james-wheeler-417074.jpg" />
      <div class="about-image-text"><h1 v-html="headerImageText"></h1></div>
    </div>
  </div>
</template>
<script>
export default {
  name: "PageImageHeaders",
  props: {
    headerImageText: String,
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
  color: #fff;
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
  object-fit: cover;
  width: 100%;
  height: 150px;
}

.about-container {
  padding: 0 18px;
}
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
}
@media only screen and (min-width: 700px) {
  img {
    height: 350px;
  }

  h1 {
    font-size: 60px;
  }
}
</style>
