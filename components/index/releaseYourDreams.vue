<template>
  <section class="wrapper">
    <v-container class="bg-img">
      <h2 class="mx-auto mb-15">Está na hora de
        <b class="text-green">realizar seus sonhos</b>
        aproveite o valor promocional em até:
      </h2>
      <client-only>
        <vac class="d-flex align-center" :end-time="endTime">
          <v-row
            style="max-width: 475px"
            class="mx-auto px-9 px-sm-0"
            slot="process"
            slot-scope="{ timeObj }"
          >
            <v-col class="pa-0">
              <div :class="$vuetify.breakpoint.smAndUp ? 'display-3' : 'title'" class="green-font-color">
                {{ `${timeObj.d}` }}
              </div>
              <div :class="$vuetify.breakpoint.smAndUp ? 'overline' : 'caption'" class="green-font-color-stt pt-2">
                Dias
              </div>
            </v-col>
            <div :class="$vuetify.breakpoint.smAndUp ? 'display-3' : 'title'" class="green-font-color">:</div>
            <v-col class="pa-0">
              <div :class="$vuetify.breakpoint.smAndUp ? 'display-3' : 'title'" class="green-font-color">
                {{ `${timeObj.h}` }}
              </div>
              <div :class="$vuetify.breakpoint.smAndUp ? 'overline' : 'caption'" class="green-font-color-stt pt-2">
                Horas
              </div>
            </v-col>
            <div :class="$vuetify.breakpoint.smAndUp ? 'display-3' : 'title'" class="green-font-color">:</div>
            <v-col class="pa-0">
              <div :class="$vuetify.breakpoint.smAndUp ? 'display-3' : 'title'" class="green-font-color">
                {{ `${timeObj.m}` }}
              </div>
              <div :class="$vuetify.breakpoint.smAndUp ? 'overline' : 'caption'" class="green-font-color-stt pt-2">
                Minutos
              </div>
            </v-col>
            <div :class="$vuetify.breakpoint.smAndUp ? 'display-3' : 'title'" class="green-font-color">:</div>
            <v-col class="pa-0">
              <div :class="$vuetify.breakpoint.smAndUp ? 'display-3' : 'title'" class="green-font-color">
                {{ `${timeObj.s}` }}
              </div>
              <div :class="$vuetify.breakpoint.smAndUp ? 'overline' : 'caption'" class="green-font-color-stt pt-2">
                Segundos
              </div>
            </v-col>
          </v-row>
          <span class="w-100" slot="finish">Done!</span>
        </vac>
      </client-only>
      <div class="container-text-button">
        <p>A X-Green te ajuda a conquistá-los</p>
        <button class="mt-5">Comece Agora</button>
      </div>
    </v-container>
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
.green-font-color {
  color: #a7e853;
  font-weight: bold;
}
.green-font-color-stt {
    color: #a7e853;
}
@media(max-width: 991px) {
  .wrapper {
    padding: 80px 30px !important;
  }
  .container-text-button {
    min-height: calc(25vh + 10rem) !important;
  }
}
.bg-img{
  background: url('/img/bg_sonhos.jpg') no-repeat center;
  background-size: contain;
}
.wrapper {
  background-color: #141414;
  padding: 50px 100px;
  text-align: center;
  min-height:  calc(70vh + 2rem);
  h2{
    font-size: 30px;
    line-height: 1.2;
    color: #ffff;
    max-width: 600px;
    font-weight: 400;
  }
  .text-green{
    color: #a7e853;
  }
}
.container-text-button {
  min-height: calc(50vh + 10rem);
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
