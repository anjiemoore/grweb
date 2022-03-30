<template>
  <div>
    <div class="card-container-outer">
      <div class="card-container-inner">
        <img class="card-image" :src="cardImage" />
        <div class="card-text">
          <h4 v-html="cardTitle"></h4>
          <p v-html="cardBody"></p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Card",
  props: {
    cardImage: Function,
    cardTitle: String,
    cardBody: String,
  },
  computed: {},
};
</script>

<style scoped>
h4 {
  /* font-size: 20px; */
  font-size: 24px;
  font-family: "Roboto";
  font-weight: bold;
}

p {
  font-size: 16px;
  font-family: "Roboto";
  color: rgb(98, 125, 152);
  line-height: 1.5;
}
.card-container-outer {
  /* display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column; */
  width: 100%;
  height: 100%;
  margin: 0 auto;
}
.card-container-inner {
  margin: 0 auto;
  display: flex;
  align-items: flex-start;
  justify-content: flex-start;
  flex-direction: column;
  width: 80%;
  height: 260px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  padding: 15px 15px 0;
}

.card-image {
  width: 25%;
  height: 30%;
  color: #34c6a6;
  fill: #34c6a6;
  filter: invert(62%) sepia(52%) saturate(492%) hue-rotate(117deg)
    brightness(94%) contrast(94%);
}
.card-text {
  text-align: left;
  padding-top: 10px;
}
img {
  width: 100%;
  height: 100%;
}
</style>
