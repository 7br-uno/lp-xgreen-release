<template>
  <div>
    <mainBanner />
    <benefits />
    <thirdBanner />
    <releaseYourDreams />
    <fifthBanner />
    <sixthBanner />
    <seventhBanner />
    <eighthBanner />
    <ninethBanner />
    <tenthBanner />
    <eleventhBanner />
    <twelfthBanner />
    <thirteenthBanner />
    <counter />
    <fifteenthBanner />
  </div>
</template>

<script>
import mainBanner from "/components/index/main_banner";
import benefits from "/components/index/benefits.vue";
import thirdBanner from "/components/index/third_banner.vue";
import releaseYourDreams from "/components/index/releaseYourDreams";
import fifthBanner from "/components/index/fifth_banner.vue";
import sixthBanner from "/components/index/sixth_banner.vue";
import seventhBanner from "/components/index/seventh_banner.vue";
import eighthBanner from "/components/index/eighth_banner.vue";
import ninethBanner from "/components/index/nineth_banner.vue";
import tenthBanner from "/components/index/tenth_banner.vue";
import eleventhBanner from "/components/index/eleventh_banner.vue";
import twelfthBanner from "/components/index/twelfth_banner.vue";
import thirteenthBanner from "/components/index/thirteenth_banner.vue";
import counter from "/components/index/counter.vue";
import fifteenthBanner from "/components/index/fifteenth_banner.vue";

export default {
  components: {
    mainBanner,
    benefits,
    thirdBanner,
    releaseYourDreams,
    fifthBanner,
    sixthBanner,
    seventhBanner,
    eighthBanner,
    ninethBanner,
    tenthBanner,
    eleventhBanner,
    twelfthBanner,
    thirteenthBanner,
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
