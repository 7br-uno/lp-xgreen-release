<template>
  <section class="wrapper pb-16">
    <v-container>
      <h2 class="text-title mx-auto">Tudo que você vê no mercado em um curso só</h2>
      <v-row class="mx-8 mt-10">
        <v-col cols="12" lg="3">
          <v-card color="grey darken-4" class="white--text rounded-xl pa-10 d-flex align-center h-414px">
          <div>
              <h2 class="display-1 font-weight-bold text-uppercase text-left">Aprenda de um jeito fácil.</h2>
              <p class="subtitle-1 text-uppercase text-left mb-0">Do basico ao avançado:</p>
          </div>
          </v-card>
          <v-card color="pink" class="white--text rounded-xl pa-10 mt-3 d-flex align-center h-130px">
            <h2 class="title text-uppercase text-center font-weight-bold mx-auto">Comece agora</h2>
          </v-card>
        </v-col>
        <v-col cols="12" sm="4" md="4" lg="3">
          <v-card color="grey darken-3" v-for="course1 in courses1" :key="course1" class="white--text rounded-xl pa-7 mb-3 d-flex align-center h-130px">
            <p class="body-2 text-uppercase text-center mb-0 font-weight-bold">{{ course1 }}</p>
          </v-card>
        </v-col>
        <v-col cols="12" sm="4" md="4" lg="3">
          <v-card color="grey darken-3" v-for="course2 in courses2" :key="course2" class="white--text rounded-xl pa-7 mb-3 d-flex align-center h-130px">
            <p class="body-2 text-uppercase text-center mb-0 font-weight-bold">{{ course2 }}</p>
          </v-card>
        </v-col>
        <v-col cols="12" sm="4" md="4" lg="3">
          <v-card color="grey darken-3" v-for="course3 in courses3" :key="course3" class="white--text rounded-xl pa-7 mb-3 d-flex align-center h-130px">
            <p class="body-2 text-uppercase text-center mb-0 font-weight-bold">{{ course3 }}</p>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  data: () => {
    return {
      courses1: [
        "Cadastros e operações nas casas de investimentos",
        "Uso correto de calculadoras",
        "Controle emocional/ Gestão de banca",
        "Estratégias conservadoras e arrojadas",
      ],
      courses2: [
        "Investimentos em futebol e outras modalidades",
        "Planejamento financeiro/juros compostos",
        "Conceitos: ODDs, ROI, Punter, Trader, etc",
        "Grupo Vip do Telegram com entradas para copiar",
      ],
      courses3: [
        "Principais mercados: resultado correto, gols, escanteios, entre outros",
        "Principais técnicas: back, lay, over, under, entre outras",
        "Alavancagem: comece com pouco dinheiro",
        "Análise pré jogo: aprenda como analisar uma partida",
      ]
    };
  },
};
</script>

<style scoped lang="scss">
.wrapper {
  background: #141414;
  text-align: center;
  width: 100%;
  .text-title{
    text-transform: uppercase;
    font-size: 35px;
    line-height: 1.2;
    color: #ffff;
    max-width: 550px;
    font-weight: 600;
  }
  .h-130px{
    height: 130px
  }
  .h-414px{
    height: 414px
  }

  .courses-container {
    width: 100%;
    display: flex;
    justify-content: center;
    li{
      list-style: none;
    }
  }
  .courses-container-cards {
    width: 33.33%;
    height: 600px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    .card {
      width: 70%;
      text-align: center;
      height: 16%;
      border-radius: 10px;
      background-color: #606060;
      padding: 6%;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      margin-bottom: 2%;
      p{
        color: #fff;
      }
    }
    .card-md {
      width: 60%;
      text-align: center;
      height: 50%;
      border-radius: 10px;
      background-color: #292828;
      padding: 4%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      margin-bottom: 2%;
      h2{
        color: #ffff;
        font-size: 2.0rem;
        text-transform: uppercase;
        text-align: initial;
      }
      p{
        color: #ffff;
        font-size: 1.0rem;
        text-transform: uppercase;
        text-align: initial;
      }
    }
    button {
    background: #F71C43;
    height: 15%;
    border: none;
    width: 60%;
    border-radius: 0.5rem;
    color: #fff;
    text-transform: uppercase;
    font-weight: 600;
    filter: drop-shadow(-1px -1px 7px #F71C43);
    cursor: pointer;
     &:hover {
      background: #c01333;
      filter: drop-shadow(-1px -1px 7px #c01333);

    }

  }
  }
}
</style>
