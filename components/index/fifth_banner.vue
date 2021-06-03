<template>
  <section class="wrapper">
    <div class="container">
      <h2 style="max-width: 830px;" :class="$vuetify.breakpoint.smAndUp ? 'display-2' : 'headline'">Você acha que está muito bom para ser verdade?</h2>
      <v-chip
        :large="$vuetify.breakpoint.smAndUp"
        class="ma-5"
        color="white font-weight-bold text-uppercase"
      >
        <v-icon
          class="pr-4"
          :large="$vuetify.breakpoint.smAndUp"
        >
          mdi-information-outline mdi-rotate-180
        </v-icon>
        Então preste atenção
        <v-icon
          class="pl-4"
          :large="$vuetify.breakpoint.smAndUp"
        >
          mdi-information-outline mdi-rotate-180
        </v-icon>
      </v-chip>
      <p class="mb-0">
        Desde 2018, a X-green conseguiu
        <b>
          lucro em mais de 95% dos dias.
        </b>
      </p>
      <p>
        <b>
          É isso mesmo! Finalizamos mais de 95% de todos os dias com lucro desde 2018.
        </b>
      </p>
    </div>
  </section>
</template>
<style scoped lang="scss">
@media(max-width: 991px) {
  .wrapper {
    padding: 30px 20px !important;
  }
}
.wrapper {
  width: 100%;
  background: #fffd00;
  padding: 6.25rem;
  .container{

    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    flex-direction: column;
    h2 {
      text-transform: uppercase;
      line-height: 1;
      font-weight: 600;
    }
    p {
    }
    .container-attention {
      width: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #ffff;
      height: 2.5rem;
      border-radius: 1.25rem;
      padding-top: 1.25rem;
      margin: 1.25rem 0 1.25rem 0;

      p{
        text-transform: uppercase;
        font-weight: 600;
      }
    }
  }
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
