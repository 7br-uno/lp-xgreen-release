<template>
  <div>
    <mainBanner />
    <benefits />
    <thirdBanner />
    <releaseYourDreams />
    <releaseYourDreamsContinuation />
    <fifthBanner />
    <sixthBanner />
    <seventhBanner />
    <eighthBanner />
    <customerOpinion />
    <tenthBanner />
    <eleventhBanner />
    <twelfthBanner />
    <counter />
    <fifteenthBanner />
  </div>
</template>

<script>
import mainBanner from "/components/index/main_banner";
import benefits from "/components/index/benefits.vue";
import thirdBanner from "/components/index/third_banner.vue";
import releaseYourDreams from "/components/index/releaseYourDreams";
import releaseYourDreamsContinuation from "/components/index/releaseYourDreamsContinuation";
import fifthBanner from "/components/index/fifth_banner.vue";
import sixthBanner from "/components/index/sixth_banner.vue";
import seventhBanner from "/components/index/seventh_banner.vue";
import eighthBanner from "/components/index/eighth_banner.vue";
import customerOpinion from "/components/index/customer_opinion";
import tenthBanner from "/components/index/tenth_banner.vue";
import eleventhBanner from "/components/index/eleventh_banner.vue";
import twelfthBanner from "/components/index/twelfth_banner.vue";
import counter from "/components/index/counter.vue";
import fifteenthBanner from "/components/index/fifteenth_banner.vue";

export default {
  components: {
    mainBanner,
    benefits,
    thirdBanner,
    releaseYourDreams,
    releaseYourDreamsContinuation,
    fifthBanner,
    sixthBanner,
    seventhBanner,
    eighthBanner,
    customerOpinion,
    tenthBanner,
    eleventhBanner,
    twelfthBanner,
    counter,
    fifteenthBanner,
  },
};
</script>

<style scoped lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

@media screen and (max-width: 1080px){
  html {
    font-size: 93.75%;
  }
}

@media screen and(max-width: 720px){
  html {
    font-size: 87.5%;
  }
}

@media screen and(max-width: 600px){
  html {
    font-size: 75%;
  }
}


</style>
