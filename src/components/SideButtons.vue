<template>
  <div class="side-ctas">
    <div class="demo-cta">
      <button class="demo">REQUEST A DEMO</button>
    </div>
    <div class="contact-cta">
      <button class="contact">CONTACT US</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "SideButtons",
};
</script>

<style scoped>
.side-ctas {
  display: none;
}
@media only screen and (min-width: 700px) {
  .side-ctas {
    display: block;
    padding: 10px 0;
    text-align: left;
    width: 230px;
  }
  .contact,
  .demo {
    width: 100%;
    font-size: 22px;
    font-family: "Impact";
    color: rgb(255, 255, 255);
    text-transform: uppercase;
    line-height: 1.5;
    text-align: center;
    border: none;
    border-radius: 10px;
    padding: 10px;
  }

  .contact {
    background-color: rgb(52, 198, 166);
  }

  .demo {
    background-color: rgb(53, 141, 221);
  }

  .demo-cta {
    padding-bottom: 10px;
  }
}
</style>
