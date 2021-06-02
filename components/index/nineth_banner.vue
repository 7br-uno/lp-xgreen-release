<template>
  <section class="wrapper">
    <h1>Veja a opinião</h1>
    <v-carousel :show-arrows="false" cycle hide-delimiter-background>
      <v-carousel-item >
          <ul class="container-chat-3">
            <li v-for="(img1, i) in imgs1" :key="i">
              <img :src="img1" alt="" class="img-chat" />
            </li>
          </ul>
      </v-carousel-item>
      <v-carousel-item>
          <ul class="container-chat-3">
            <li v-for="(img2, i) in imgs2" :key="i">
              <img :src="img2" alt="" class="img-chat" />
            </li>
          </ul>

      </v-carousel-item>
    </v-carousel>
  </section>
</template>

<script>
export default {
  data() {
    return {
      imgs1: ["/img/chat01.png", "/img/chat02.png", "/img/chat03.png"],
      imgs2: ["/img/chat04.png", "/img/chat05.png", "/img/chat06.png"],
    };
  },
};
</script>


<style scoped lang="scss">
.wrapper {
  background: #000000;
  text-align: center;
  padding: 100px;
  h1 {
    color: #ffffff;
  }
}
.container-chat-3 {
  width: 50%;
  display: flex;
  /* flex-wrap: wrap; */
  justify-content: center;
  align-items: center;
  align-items: center;
  background: #000000;
}
.img-chat {
  width: 25%;
  height: 40%;
}
.v-responsive__content {
  max-width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
