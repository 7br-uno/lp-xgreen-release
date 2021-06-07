<template>
  <section class="wrapper pt-16">
    <h2
      :class="$vuetify.breakpoint.smAndUp ? '' : 'display-1 font-weight-bold'"
      class="mt-10 mx-auto"
    >
      E mais: Temos o Robozão absurdamente bom!
    </h2>
    <p class="text-green">(E que não foi barato)</p>
    <div class="container">
      <v-row>
        <v-col cols="12" md="6" lg="4">
          <div class="robozao_strategist mx-auto">
            <div>
              <img src="/img/icone_robozao_televisao_01.png" alt="" />
              <p>
                Uma inteligência artificial, apelidada de Robozão, indica as
                nelhores entradas e jogos da nossa estratégia vencedora desde
                2018
              </p>
            </div>
          </div>
        </v-col>
        <v-col cols="12" md="6" lg="4">
          <div class="robozao_strategist mx-auto">
            <div>
              <img src="/img/icone_robozao_uniao_02.png" alt="" />
              <p>
                A partir da análise do Robozão, nossa equipe de especialistas
                avalia as partidas e indica as melhores entradas do mercado para
                você replicar.
              </p>
            </div>
          </div>
        </v-col>
        <v-col cols="12" md="12" lg="4">
          <div class="robozao_strategist mx-auto">
            <div>
              <img src="/img/icone_robozao_bola_03.png" alt="" />
              <p>
                A união dos nossos tipster com o Robozão é o que faz da nossa
                metodologia única, um sucesso.
              </p>
            </div>
          </div>
        </v-col>
      </v-row>
    </div>
  </section>
</template>
<style scoped lang="scss">
@media (max-width: 991px) {
  .wrapper {
    padding: 30px 20px !important;
  }
}
.wrapper {
  background: #191919;
  padding: 50px;
  text-align: center;
  h2 {
    color: #ffff;
    font-size: 2.5rem;
    text-transform: uppercase;
    line-height: 1;
    max-width: 600px;
  }
  .text-green {
    color: #a7e853;
    font-size: 18px;
    text-transform: uppercase;
    line-height: 2;
  }
  .container {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    margin-top: 60px;

    .robozao_strategist {
      width: 350px;
      img {
        max-width: 100px;
        padding-bottom: 1rem;
      }
      p {
        font-size: 1rem;
        text-align: initial;
        color: #ffff;
      }
    }
  }
}
</style>
