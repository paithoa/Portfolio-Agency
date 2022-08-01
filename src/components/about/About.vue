<template>
  <div class="about-page">
    <div class="rn-story-area d-flex bg_color--3" id="about">
      <div
        class="rn-story-left w-50 rn-story-bg-wrapper"
        :style="{ backgroundImage: 'url(' + aboutSrc + ')' }"
      ></div>
      <div class="rn-story-right w-50 d-flex align-items-center">
        <div
          class="story-style--3 story-content text-left rn-plr--160 section-ptb-xl"
        >
          <div class="content text-left">
            <h1 style="font-size:32px">
              Our Services
            </h1>
            <br>
            <p style="font-size:24px">
              · Website Design & Development
            </p>
            <p style="font-size:24px">
          · Web Conversion & CRO Strategies
            </p>
            <div
              class="story-btn  wow newFadeInUp"
              data-wow-duration="1s"
              data-wow-delay="1000ms"
            >
             
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- End Story Area -->
    <!-- Start Skill Area -->
    <div class="rn-skill-area home-one-skill d-flex bg_color--3" id="skill">
      <div class="rn-skill-right w-50 d-flex align-items-center">
        <div class="text-left rn-skill rn-plr section-ptb-xl">
            <div class="content text-left">
           
            <p style="font-size:24px">
              · Advanced Custom Web Solutions
            </p>
            <p style="font-size:24px">
· Web API Integration Solutions            </p>
            <div
              class="story-btn  wow newFadeInUp"
              data-wow-duration="1s"
              data-wow-delay="1000ms"
            >
            
            </div>
          </div>
        </div>
      </div>
      <div
        class="rn-skill-left w-50 rn-skill-bg-wrapper"
        :style="{ backgroundImage: 'url(' + skillSrc + ')' }"
      ></div>
    </div>
    <!-- End Skill Area -->
  </div>
</template>

<script>
  export default {
    data() {
      return {
        aboutSrc: require("../../assets/img/portfolio/about-image.jpg"),
        skillSrc: require("../../assets/img/portfolio/my-skill.jpg"),
      };
    },
  };
</script>

<style lang="scss" scoped>
  .about-page {
    .rn-skill-right {
      @media only screen and (max-width: 767px) {
        order: 2;
      }
    }
  }
</style>
