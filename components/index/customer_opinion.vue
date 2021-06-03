<template>
  <section class="wrapper">
    <h1>Veja a opinião dos nossos clientes</h1>
    <v-carousel :show-arrows="false" cycle hide-delimiter-background>
      <v-carousel-item>
        <div class="container-chat-3">
          <div v-for="(img1, i) in imgs1" :key="i">
            <img :src="img1" alt="" class="img-chat" />
          </div>
        </div>
      </v-carousel-item>
      <v-carousel-item>
        <div class="container-chat-3">
          <div v-for="(img2, i) in imgs2" :key="i">
            <img :src="img2" alt="" class="img-chat" />
          </div>
        </div>
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
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 50px;
  h1 {
    color: #ffffff;
    font-size: 60px;
  }
}
.container-chat-3 {
  width: 100%;
  display: flex;
  justify-content: center;
  flex-direction: row;
  align-items: center;
  padding-top: 100px;
}
.img-chat {
  width: 50%;
}

@media (max-width: 991px) {
  .wrapper {
    padding: 50px 0px;
    h1 {
      font-size: 36px;
    }
  }
  .img-chat {
  width: 150px;
  margin-right: 4px;
}
}

@media (max-width: 600px) {

.container-chat-3 {
  flex-direction: column;
}
.img-chat {
  width: 80%;
}
}
</style>
