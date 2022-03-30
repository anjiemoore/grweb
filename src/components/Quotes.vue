<template>
  <div class="quote-container">
    <div class="quote-inner">
      <template v-for="quotes in quoteArray" :key="quotes.quote">
        <div class="quote-image">
          <img class="quote-logos" :alt="quotes.alt" :src="quotes.image" />
        </div>
        <div class="quote">
          <blockquote>
            <p>{{ quotes.quote }}</p>
            <div class="quote-credits">
              <figcaption>{{ quotes.credit }} <br /></figcaption>
            </div>
            <p class="quote-position">{{ quotes.position }}</p>
          </blockquote>
          <div class="quote-arrows">
            <div class="quote-arrows-inner">
              <button class="left-arrow">
                <img src="../assets/svgs/left-arrow.svg" />
              </button>
              <button class="right-arrow">
                <img src="../assets/svgs/right-arrow.svg" />
              </button>
            </div>
          </div>
        </div>
      </template>
    </div>
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
          image: require(`@/assets/companies/Pinehurst.png`),
          alt: "Pinehurst logo",
          credit: "Scott Brewton",
          position:
            "Senior Vice President & General Manager, Pinehurst Resort & Spa",
        },
        // {
        //   quote:
        //     "Their loyalty-based feedback system is a great fit with our priorities. We definitely give Guest Research a ‘10’.",
        //   image: require(`@/assets/companies/Greenbrier.png`),

        //   alt: "Greenbrier logo",
        //   credit: "Jeff Kmiec",
        //   position: "President & Managing Director, The Greenbrier",
        // },
        // {
        //   quote:
        //     "Guest Research conducts for Crystal Mountain Resort satisfaction research for our guests, meeting planners and employees. The research is not only more comprehensive than what other companies provide, but Guest Research’s team provides the consultative support we need to maximize the value of the information. Most importantly, the research has helped us achieve real increases in satisfaction, revenues and profits.",
        //   image: require(`@/assets/companies/Crystal.png`),

        //   alt: "Crystal Mountain logo",
        //   credit: "Chris MacInnes",
        //   position: "Senior Vice President, Crystal Mountain Resort",
        // },
        // {
        //   quote:
        //     "We have partnered for many years with Guest Research. The satisfaction and loyalty research they conduct with us for our guests, homeowners and employees is critical to our company’s growth.",
        //   image: require(`@/assets/companies/Eastwest.png`),

        //   alt: "East West logo",
        //   credit: "Peter Dann, ",
        //   position: "Executive Vice President, East West Resorts",
        // },
        // {
        //   quote:
        //     "NPS is one of the most critical financial metrics our three resorts use, and it has had a tremendous impact on our revenue growth, with the enhanced guest loyalty positioning us well for the future. It has been firmly integrated into our culture.",
        //   image: require(`@/assets/companies/Fairbank.png`),

        //   alt: "Fairbank Group logo",
        //   credit: "Tyler Fairbank, ",
        //   position: "CEO, The Fairbank Group",
        // },
        // {
        //   quote:
        //     "Guest Research’s Homeowner NPS research has provided us with valuable feedback from our owners, which is helping us better manage our partnerships. The insight into our owners’ opinions will most certainly help us increase their loyalty and referrals.",
        //   image: require(`@/assets/companies/Parrish.png`),
        //   alt: "The Parrish Collection logo",
        //   credit: "Jonathan “JP” Parrish, ",
        //   position:
        //     "President and Principal Broker, The Parrish Collection Kauai",
        // },
      ],
    };
  },
  methods: {},
  computed: {},
};
</script>

<style scoped>
.quote-container {
  width: 100%;
  height: 100%;
}

.quote-inner {
  flex-direction: column;
  display: flex;
}
.quote-logos {
  width: 80%;
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

.quote-arrows {
  width: 50%;
  display: flex;
  flex-direction: row;
}

button {
  background: transparent;
  border: none;
  width: 40px;
}

button img {
  width: 20px;
}

@media only screen and (min-width: 700px) {
  .quote-container {
    width: 70%;
    /* flex-direction: row;
    align-items: baseline; */
  }
  .quote-inner {
    flex-direction: row;
    align-items: center;
    justify-content: center;
  }
  .quote-image {
    min-width: 50%;
  }
  .quote {
    flex-direction: column;
  }
  .quote-arrows {
    align-content: flex-start;
    justify-content: flex-start;
    padding: 10px 0 0 20px;
  }
}
</style>
