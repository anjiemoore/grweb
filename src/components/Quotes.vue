<template>
  <div class="quote-container">
    <template v-for="quotes in quoteArray" :key="quotes.quote">
      <img class="quote-logos" :alt="quotes.alt" :src="quotes.image" />
      <blockquote>
        <p>{{ quotes.quote }}</p>
        <div class="quote-nav">
          <div class="quote-credits">
            <figcaption>{{ quotes.credit }} <br /></figcaption>
          </div>
          <div class="quote-arrows">
            <button
              class="quote-arrow-left"
              src="../assets/svgs/left-arrow.svg"
              alt=""
            />
          </div>
        </div>
        <p class="quote-position">{{ quotes.position }}</p>
      </blockquote>
    </template>
  </div>
</template>

<script>
export default {
  name: "Quotes",
  data() {
    return {
      quoteArray: [
        {
          quote:
            "We highly recommend Guest Research's Net Promoter System. Their software is powerful, yet easy to use, and their team has worked closely with us to significantly increase our guest and meeting planner satisfaction and loyalty.",
          image: "../assets/companies/crystal-mtn.jpg",
          alt: "Pinehurst logo",
          credit: "Scott Brewton",
          position:
            "Senior Vice President & General Manager, Pinehurst Resort & Spa",
        },
        {
          quote:
            "Their loyalty-based feedback system is a great fit with our priorities. We definitely give Guest Research a ‘10’.",
          image:
            "https://image.freepik.com/free-photo/image-human-brain_99433-298.jpg",
          alt: "Greenbrier logo",
          credit: "Jeff Kmiec",
          position: "President & Managing Director, The Greenbrier",
        },
        {
          quote:
            "Guest Research conducts for Crystal Mountain Resort satisfaction research for our guests, meeting planners and employees. The research is not only more comprehensive than what other companies provide, but Guest Research’s team provides the consultative support we need to maximize the value of the information. Most importantly, the research has helped us achieve real increases in satisfaction, revenues and profits.",
          image:
            "https://image.freepik.com/free-photo/image-human-brain_99433-298.jpg",
          alt: "Crystal Mountain logo",
          credit: "Chris MacInnes",
          position: "Senior Vice President, Crystal Mountain Resort",
        },
        {
          quote:
            "We have partnered for many years with Guest Research. The satisfaction and loyalty research they conduct with us for our guests, homeowners and employees is critical to our company’s growth.",
          image:
            "https://image.freepik.com/free-photo/image-human-brain_99433-298.jpg",
          alt: "East West logo",
          credit: "Peter Dann, ",
          position: "Executive Vice President, East West Resorts",
        },
        {
          quote:
            "NPS is one of the most critical financial metrics our three resorts use, and it has had a tremendous impact on our revenue growth, with the enhanced guest loyalty positioning us well for the future. It has been firmly integrated into our culture.",
          image:
            "https://image.freepik.com/free-photo/image-human-brain_99433-298.jpg",
          alt: "Fairbank Group logo",
          credit: "Tyler Fairbank, ",
          position: "CEO, The Fairbank Group",
        },
        {
          quote:
            "Guest Research’s Homeowner NPS research has provided us with valuable feedback from our owners, which is helping us better manage our partnerships. The insight into our owners’ opinions will most certainly help us increase their loyalty and referrals.",
          image:
            "https://image.freepik.com/free-photo/image-human-brain_99433-298.jpg",
          alt: "The Parrish Collection logo",
          credit: "Jonathan “JP” Parrish, ",
          position:
            "President and Principal Broker, The Parrish Collection Kauai",
        },
      ],
    };
  },
};
</script>

<style scoped>
.quote-container {
  width: 100%;
  height: 100%;
}
.quote-logos {
  width: 50%;
}

blockquote {
  position: relative;
}
blockquote::before {
  content: "\201C";
  color: #358ddd;
  font-size: 60px;
  font-family: sans-serif;
  position: absolute;
  z-index: 1;
  left: 0px;
  top: -11px;
}
p {
  font-size: 16px;
  font-family: "Roboto";
  color: rgb(98, 125, 152);
  font-style: italic;
  line-height: 1.333;
  text-align: left;
  padding: 0 30px;
}
figcaption {
  font-size: 19px;
  font-family: "Roboto";
  color: rgb(64, 137, 201);
  font-weight: bold;
  line-height: 1;
  text-align: left;
  padding: 15px 30px 0;
}
.quote-position {
  font-size: 16px;
  font-family: "Roboto";
  color: rgb(98, 125, 152);
  font-style: italic;
  line-height: 1.333;
  text-align: left;
  padding: 0 30px;
}
.quote-nav {
  display: flex;
  flex-direction: row;
  align-items: baseline;
}
.quote-arrows {
  width: 20%;
}
</style>
