<template>
  <div class="footer-container">
    <div class="footer-cta-logo">
      <button class="footer-cta">READY TO GET STARTED?</button>
      <img src="../assets/GuestResearchLogo.png" class="footer-logo" />
    </div>
    <div class="footer-contact-container">
      <div class="footer-mail">
        <img src="../assets/mail.png" class="footer-icons" />
        <a href="mailto=info@guestresearch.com" class="links"
          >info@guestresearch.com</a
        >
      </div>
      <div class="footer-phone">
        <img src="../assets/phone.png" class="footer-icons phone" />
        <a href="tel=3034889808" class="links">(303) 488-9808</a>
      </div>
    </div>
    <div class="footer-address">
      <p>5500 S. Krameria Street | Greenwood Village, CO 80111</p>
    </div>
    <div class="footer-menu">
      <router-link to="/">HOME</router-link>
      <router-link to="/about">WHO WE ARE</router-link>
      <router-link to="/different">HOW WE’RE DIFFERENT</router-link>
      <router-link to="">FEATURES</router-link>
      <router-link to="">THE TEAM</router-link>
      <router-link to="">GET IN TOUCH</router-link>
    </div>
    <div class="footer-copyright">
      <p>© Guest Research, Inc.<br />All Right Reserved Privacy Policy</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
.footer-container {
  width: 100%;
  padding: 0 18px;
  /* position: fixed;
  left: 0;
  bottom: 0;
  right: 0; */
}
.footer-cta-logo {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.footer-cta {
  width: 100%;
  font-size: 22px;
  font-family: "Impact";
  color: rgb(255, 255, 255);
  text-transform: uppercase;
  line-height: 1.5;
  text-align: center;
  border: none;
  border-radius: 10px;
  background-color: rgb(52, 198, 166);
  padding: 15px 15px;
}
.footer-logo {
  padding: 30px 26px 15px 0;
  width: 200px;
}

.footer-contact-container {
  display: flex;
  justify-content: space-around;
  width: 100%;
}
.footer-icons {
  width: 27px;
  padding: 0 7px;
}

.footer-address {
  padding: 5px 0 12px 0;
}
.footer-menu {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;
  /* padding: 0 21px; */
}

.links {
  letter-spacing: 0px !important;
}
a {
  letter-spacing: 1.3px;
  padding: 5px 0;
}
.footer-copyright {
  padding: 20px;
}

.links,
a,
p {
  font-size: 12px;
  font-family: "Open Sans";
  color: rgb(51, 104, 155);
  font-weight: bold;
  text-transform: uppercase;
  line-height: 1.2;
  text-align: center;
  text-decoration: none;
}
</style>
>
