<template>
  <section class="wrapper">
    <h2>Está na hora de
      <b class="text-green">realizar seus sonhos</b>
      aproveite o valor promocional em até:
    </h2>
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
    <div class="container-text-button">
      <p>A X-Green te ajuda a conquistá-los</p>
      <button>Comece Agora</button>
    </div>
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
.font-weight-bold {
  color: #a7e853;
  font-size: 80px !important;
}
.overline {
    color: #a7e853;
    padding-top: 1rem;
}
.wrapper {
  background: url('/img/bg_sonhos.jpg');
  padding: 100px;
  text-align: center;
  background-size: cover;
  background-position: center;
  background-repeat:no-repeat;
  min-height:  calc(100vh + 10rem);
  h2{
    font-size: 30px;
    line-height: 1.2;
    color: #ffff;
    padding: 0 20rem 5rem 20rem;
    font-weight: 400;
  }
  .text-green{
    color: #a7e853;
  }
}
.container-text-button {
  min-height: calc(100vh + 10rem);
  display: flex;
  justify-content: flex-end;
  align-items: center;
  flex-direction: column;
  p {
    color: #fff;
  }
  button {
    background: #F71C43;
    height: 3rem;
    border: none;
    width: 16rem;
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
</style>
