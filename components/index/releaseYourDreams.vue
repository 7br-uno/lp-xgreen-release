<template>
  <section class="wrapper">
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
  background: #131313;
  padding: 100px;
  text-align: center;
  height: 80vh;
}
</style>
