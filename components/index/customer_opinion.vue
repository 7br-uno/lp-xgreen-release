<template>
  <section class="wrapper">
    <h1 class="text-uppercase">Se liga na opinião da galera</h1>
    <v-carousel height="350" class="d-block d-sm-none" :show-arrows="false" hide-delimiter-background>
      <v-carousel-item v-for="(single, i) in all" :key="i">
        <div class="mt-8">
          <img :src="single" alt="" class="img-chat" />
        </div>
      </v-carousel-item>
    </v-carousel>
    <v-carousel class="d-none d-sm-block" :show-arrows="false" cycle hide-delimiter-background>
      <v-carousel-item>
        <div class="container-chat-3">
          <div v-for="(img1, i) in imgs1" :key="i">
            <img :src="img1" alt="Opinião dos nossos clientes" class="img-chat" />
          </div>
        </div>
      </v-carousel-item>
      <v-carousel-item>
        <div class="container-chat-3">
          <div v-for="(img2, i) in imgs2" :key="i">
            <img :src="img2" alt="Opinião dos nossos clientes" class="img-chat" />
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
      all: ["/img/chat01.png", "/img/chat02.png", "/img/chat03.png", "/img/chat04.png", "/img/chat05.png", "/img/chat06.png"],
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
  width: 60%;
  display: flex;
  justify-content: center;
  flex-direction: row;
  align-items: center;
  padding-top: 80px;
  margin: 0 auto;
}
.img-chat {
  width: 85%;
}

@media (min-width: 992px) {
  .img-chat {
    width: 250px;
    margin: 0 15px;
  }
}

@media (max-width: 991px) {
  .wrapper {
    padding: 50px 0px;
    h1 {
      font-size: 36px;
    }
  }
  .img-chat {
    width: 190px;
    margin: 0 15px;
  }
}
</style>
