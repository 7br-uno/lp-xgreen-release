<template>
  <section class="wrapper">
    <v-row>
      <v-col class="d-flex align-center" cols="12" sm="7" md="6" offset-md="1">
        <div>
          <img class="img-notebook" src="/img/bg_note.png" alt="notebook">
          <v-row class="my-card">
            <v-col class="red darken-4 bd-radius-lt d-flex align-center" cols="2">
              <v-icon class="mx-auto" color="white">
                mdi-soccer
              </v-icon>
            </v-col>
            <v-col class="red text-left bd-radius-rt-rb" cols="10">
              <div class="font-weight-bold white--text">
                Vai dar certo mesmo que você não entenda nada de futebol
              </div>
              <div class="caption white--text">
                Será fácil nós te <span class="font-weight-bold">ensinamos tudo.</span>
              </div>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <v-col cols="12" sm="5" md="4">
        <div class="title white--text text-left">
          Aqui você tem o
        </div>
        <div class="display-3 primary--text font-weight-black text-left overing">
          curso mais completo
        </div>
        <div class="slab">
          Assim como nós, transforme sua vida!
        </div>
        <div
          v-for="(benefit, i) in benefits"
          :key="i"
          :class="i + 1 === benefits.length ? 'bd-none' : ''"
          class="border-bot-pers py-3 grey--text text-left"
        >
          {{benefit}}
        </div>
        <v-btn
          class="mt-2"
          color="pink"
          elevation="2"
          dark
          x-large
        >
          Comece agora
        </v-btn>
      </v-col>
    </v-row>
  </section>
</template>

<script>
export default {
  data: () => {
    return {
      benefits:[
        'Ganhe uma renda extra todo mês',
        'Melhore de vida e de patamar financeiro',
        'Trabalhe de qualquer lugar. Basta um celular, internet e determinação',
        'Comece com qualquer valor',
        'Monte seu proprio horário. Bastam poucos minutos por dia'
      ]
    }
  }
}
</script>

<style scoped lang="scss">
  .wrapper {
    background: #131313;
    padding: 100px;
    text-align: center;
    .conatiner{
      width: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 80vh;
    }
  }

  .border-bot-pers{
    border-bottom: 1px dashed lightgrey;
  }
  .bd-none{
    border: none !important;
  }

  .slab{
    background: grey;
    color: white;
    padding: 10px;
    margin-bottom: 18px;
    margin-top: -8px;
    transform: rotate(
        355deg
    );
  }

  .overing{
    z-index: 1;
    position: relative;
  }

  .my-card{
    max-width: 350px;
    margin: 0 auto;
  }
  .bd-radius-lt{
    border-top-left-radius: 25px;
  }
  .bd-radius-rt-rb{
    border-top-right-radius: 25px;
    border-bottom-right-radius: 25px;
  }
  .img-notebook{
    width: 95%;
    margin-bottom: -20px;
    position: relative;
    z-index: 2;
  }
</style>
