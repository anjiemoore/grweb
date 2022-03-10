<template>
  <div>
    <div class="about-image-container">
      <img src="../assets/svgs/left-arrow.svg" />
      <div class="about-image-text" v-html="headerImageText"></div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Card",
  props: {
    headerImageText: String,
  },
};
</script>

<style></style>
