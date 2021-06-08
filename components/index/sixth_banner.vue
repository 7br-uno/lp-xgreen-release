<template>
  <section class="wrapper">
    <v-container>
      <div
        :class="$vuetify.breakpoint.mdAndUp ? 'display-2' : 'display-1'"
        class="mt-15 pt-10 primary--text font-weight-black text-center overing text-uppercase"
      >
        Rendimento desde 2018
      </div>
      <v-row class="white--text graph-div mb-16">
        <v-col cols="12" md="3" :order="$vuetify.breakpoint.mdAndUp ? 'last' : ''">
          <div class="grey d-flex align-center text-center rounded-lg pa-3 mt-10">
            <v-icon color="white" left>
              mdi-download
            </v-icon>
            <span class="caption lh-12">
            Baixe nossos resultados agora!
            </span>
          </div>
          <div class="black text-center rounded-lg pa-3 mt-3">
            <div class="font-weight-bold">
              <div class="d-flex align-center text-center">
                <div style="background-color: #ff8600" class="rounded-lg color-indice ml-auto"></div>
                <div class="ml-2 mr-auto">Poupança</div>
              </div>
            </div>
            <div class="font-weight-bold">
              <div class="d-flex align-center text-center">
                <div style="background-color: #00f1ea" class="rounded-lg color-indice ml-auto"></div>
                <div class="ml-2 mr-auto">Ibovespa</div>
              </div>
            </div>
            <div class="font-weight-bold">
              <div class="d-flex align-center text-center">
                <div style="background-color: #b000ff" class="rounded-lg color-indice ml-auto"></div>
                <div class="ml-2 mr-auto">Bitcoin</div>
              </div>
            </div>
            <div class="font-weight-bold">
              <div class="d-flex align-center text-center">
                <div style="background-color: #00ff00" class="rounded-lg color-indice ml-auto"></div>
                <div class="ml-2 mr-auto">X-GREEN</div>
              </div>
            </div>
          </div>
          <div class="black text-center rounded-lg pa-3 mt-3">
            <div class="font-weight-bold">
              Rendimento anual X-GREEN
            </div>
            <div class="font-weight-bold ml-4">
              2018 <span class="yellow--text ml-2">+ 506%*</span>
            </div>
            <div class="font-weight-bold ml-4">
              2019 <span class="yellow--text ml-2">+ 808%</span>
            </div>
            <div class="font-weight-bold ml-4">
              2020 <span class="yellow--text ml-2">+ 936%</span>
            </div>
            <div class="font-weight-bold ml-4">
              2021 <span class="blue--text darken-1 ml-2">+ 276%**</span>
            </div>
            <div class="caption text-left px-3 mt-1">Estratégia arrojada</div>
          </div>
          <div class="caption text-center mt-3">
            <div>
              * Maio até dezembro
            </div>
            <div class="blue--text darken-1">
              ** Até o final de março
            </div>
          </div>
        </v-col>
        <v-col cols="12" md="9" :order="$vuetify.breakpoint.mdAndUp ? 'first' : ''">
          <!--https://www.chartjs.org/docs/latest/charts/line.html-->
          <line-chart :chart-data="datacollection" :options="chartOptions" class="graph mx-auto my-0 my-md-10"></line-chart>
        </v-col>
      </v-row>
      <div v-if="!$vuetify.breakpoint.mdAndUp" style="height: 445px"></div>
      <div class="text-center white--text font-weight-bold headline mb-15 pt-10 text-uppercase">
        Lembre-se: Você vai poder copiar a nossa estratégia e lucrar mais
      </div>
    </v-container>
    <div class="text-center">
      <v-btn
        x-large
        color="pink"
        dark
        class="desloc_vert"
      >
        <b>QUERO LUCRAR AGORA</b>
      </v-btn>
    </div>
  </section>
</template>

<script>
import LineChart from '@/components/LineChart'
export default {
  components: {
    LineChart
  },
  data () {
    return {
      datacollection: null,
      chartOptions:{
        responsive: true,
        maintainAspectRatio: false,
        legend: {
          display: false
        }
      }
    }
  },
  mounted () {
    this.fillData()
  },
  methods: {
    fillData () {
      this.datacollection = {
        labels: ['', '2018', '2019', '2020', '2021'],
        datasets: [
          {
            label: 'X-GREEN',
            tension: 0,
            fill: false,
            borderColor: '#00ff00',
            borderWidth: 6,
            data: [2, 60, 80, 100, 60]
          },
          {
            label: 'Bitcoin',
            tension: 0,
            fill: false,
            borderColor: '#b000ff',
            borderWidth: 5,
            data: [1, 30, 45, 44, 30],
          },
          {
            label: 'Ibovespa',
            tension: 0,
            fill: false,
            borderColor: '#00f1ea',
            borderWidth: 5,
            data: [0, 25, 30, 15, 9],
          },
          {
            label: 'Poupança',
            tension: 0,
            fill: false,
            borderColor: '#ff8600',
            borderWidth: 5,
            data: [0, 15, 13, 14, 10],
          },
        ]
      }
    }
  }
}
</script>

<style scoped lang="scss">
.wrapper {
  background: #1F1F1F;
}
.graph-div{
  height: 500px;
  margin-bottom: 50px;
}
.graph {
  max-width: 800px;
  background: #070707;
  border-radius: 10px;
  padding: 40px;
}
.desloc_vert{
  margin-bottom: -28px;
}
.lh-12{
  line-height: 1.1;
}
.color-indice{
  height: 10px;
  width: 20px;
}
</style>
