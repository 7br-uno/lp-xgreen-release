<template>
  <section class="wrapper pa-8 white--text">
    <v-row>
      <v-col class="d-flex align-center" cols="12" sm="6" md="4" offset-md="2">
        <client-only>
          <vac class="w-100" :end-time="endTime">
            <v-row
              class="w-100"
              slot="process"
              slot-scope="{ timeObj }"
            >
              <v-col class="pa-0">
                <div class="display-1 font-weight-bold">
                  {{ `${timeObj.d}` }}
                </div>
                <div class="overline">
                  Dias
                </div>
              </v-col>
              <div class="display-1 font-weight-bold">:</div>
              <v-col class="pa-0">
                <div class="display-1 font-weight-bold">
                  {{ `${timeObj.h}` }}
                </div>
                <div class="overline">
                  Horas
                </div>
              </v-col>
              <div class="display-1 font-weight-bold">:</div>
              <v-col class="pa-0">
                <div class="display-1 font-weight-bold">
                  {{ `${timeObj.m}` }}
                </div>
                <div class="overline">
                  Minutos
                </div>
              </v-col>
              <div class="display-1 font-weight-bold">:</div>
              <v-col class="pa-0">
                <div class="display-1 font-weight-bold">
                  {{ `${timeObj.s}` }}
                </div>
                <div class="overline">
                  Segundos
                </div>
              </v-col>
            </v-row>
            <span class="w-100" slot="finish">Done!</span>
          </vac>
        </client-only>
      </v-col>
      <v-col class="d-flex align-center" cols="12" sm="6" md="4">
        <span>
          Não perca mais tempo
        </span>
        <v-btn
          depressed
          class="ml-6 white--text"
          color="red darken-4"
        >
          Comece agora
        </v-btn>
      </v-col>
    </v-row>
  </section>
</template>
<script>
export default {
  mounted() {
    console.log(this.endTime)
  },
  computed:{
    endTime: () => {
      return new Date(2021, 5, 15);
    }
  }
}
</script>
<style scoped lang="scss">
.wrapper {
  background: #F71C43;
  padding: 100px;
  text-align: center;
}
.w-100{
  width: 100%;
}
</style>
