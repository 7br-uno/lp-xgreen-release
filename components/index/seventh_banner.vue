<template>
  <section class="wrapper">
    <v-container>
      <v-row>
        <v-col class="text-right text-sm-left" cols="12" md="6" offset-md="6">
          <div class="f-container">
            <p class="first font-weight-bold">Agora você pode estar pensando:<br>como isso é possível?</p>
            <h2 :class="$vuetify.breakpoint.smAndUp ? '' : 'display-1 font-weight-bold'">Nós temos<br>os melhores especialistas...</h2>
            <p class="second mt-2">Mas não nascemos prontos!</p>
          </div>
          <p class="white--text pl-md-15 ml-auto ml-sm-0 p-subtitle">
            Operamos desde 2015. Fizemos <b>muitos</b> testes, erramos várias vezes,
            até chegar nesta estratégia <b>sólida e lucrativa.</b>
          </p>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>
<style scoped lang="scss">
@media(max-width: 991px) {
  .wrapper {
    padding: 50px 20px !important;
  }
}
.wrapper {
  width: 100%;
  background-image: url("/img/bg_jigsaw.jpg");
  background-color: #070707;
  background-position: center;
  padding: 100px;
  display: flex;
  justify-content: center;
  align-items: flex-end;
  flex-direction: column;
  .f-container {

    .first{
      color: #fff;
      font-size: 18px;
      text-transform: uppercase;

    }
    h2 {
      color: #a7e853;
      font-size: 50px;
      text-transform: uppercase;
      line-height: 1;
    }
    .second {
      color:  #a7e853;
      font-size: 18px;
      text-transform: uppercase;
    }
  }
  .s-container {

    p {
      color: #fff;
      font-size: 20px;
    }
  }
}
.p-subtitle{
  max-width: 255px;
}
</style>
