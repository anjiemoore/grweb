<template>
  <div>
    <div class="card-container">
      <img class="card-image" :src="cardImage" />
      <div class="card-text">
        <h5 class="card-title" v-html="cardTitle"></h5>
        <p class="card-body" v-html="cardBody"></p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Card",
  props: {
    cardImage: String,
    cardTitle: String,
    cardBody: String,
  },
};
</script>

<style></style>
