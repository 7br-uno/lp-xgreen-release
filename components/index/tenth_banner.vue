<template>
  <section class="wrapper">
    <v-container>
      <div class="title-bonus mx-auto mb-15">
        <h2 :class="$vuetify.breakpoint.smAndUp ? '' : 'display-1 font-weight-bold'">Bônus!</h2>
        <p>
          E garantindo a sua vaga no
          <b>período promocional você ganha mais 8 bônus:</b>
        </p>
      </div>
      <v-row class="mb-10">
        <v-col
          cols="12"
          sm="6"
          md="3"
          v-for="cardBonus in cardsBonus"
          :key="cardBonus.img"
          class="list-cards d-flex"
        >
          <div class="mx-auto">
            <div
              class="container-bonus"
              :style="`background: url(${cardBonus.img}); background-size: cover; background-position: center`"
            >
              <span></span>
              <h2>
                {{ cardBonus.titulo }}
              </h2>
            </div>
            <div class="container-p py-4">
              <span class="p-green">{{ cardBonus.precoDe }}</span>
              <span class="white--text px-2">|</span>
              <span class="p-red font-weight-bold">
                {{ cardBonus.precoPor }}
              </span>
            </div>
            <p class="p-desc">
              {{ cardBonus.description }}
            </p>
          </div>
        </v-col>
      </v-row>
      <v-container>
        <div class="container-adesao">
          <div class="border-green">
            <div class="c-text-div pa-3">
              <div class="h2-c-green text-uppercase">
                <div :class="$vuetify.breakpoint.smAndUp ? 'display-1' : 'headline'" class="font-weight-bold">
                  São mais de R$ 7 mil em bônus,
                </div>
                <div :class="$vuetify.breakpoint.smAndUp ? 'headline' : 'subtitle-1'" class="font-weight-medium">
                  + acesso à metodologia exclusiva fast green ®
                </div>
              </div>
              <div class="p-c-green text-lg-h5 text-sm-body-2">
                E você não vai pagar por nenhum deles!
              </div>
            </div>
          </div>
          <div class="background-pink py-12">
            <div class="c-text-div">
              <div :class="$vuetify.breakpoint.smAndUp ? 'headline' : ''" class="text-lg-h5 text-bp">
                <span class="text-white">E vamos além,</span> vamos te dar
                <span class="text-black">R$ 3.000,00</span> de desconto no curso
                <b class="text-brackground">Até dia 25/04</b>
              </div>
            </div>
          </div>
          <v-btn
            x-large
            color="white"
            class="pink--text btn-pers"
          >
            <b>+ Adesão zero</b>
          </v-btn>
        </div>
      </v-container>
      <!-- ========================================================= -->
      <!-- <section class="container-cards">
        <div class="c-adesao">
          <div class="c-green">
            <h4>Adesão: R$ 399</h4>
          </div>
          <div class="c-grey">
            <div class="c-border">
              <h2 class="h2-mensal">Mensal</h2>
              <h1 class="h1-green">299,00</h1>
            </div>
          </div>
          <div class="c-list-desc">
            <ul class="desc-card">
              <li v-for="(listItem1, i) in listItems1" :key="i">
                <v-icon small color="grey darken-2"> mdi-check-bold </v-icon>
                {{ listItem1.desc }}
              </li>
            </ul>

            <button>Quero começar</button>
          </div>
        </div>
      </section> -->
    </v-container>
  </section>
</template>

<script>
export default {
  data: () => {
    return {
      cardsBonus: [
        {
          img: "/img/bonus1.jpg",
          titulo: "Acesso à metodologia X-green",
          precoDe: "R$1.599",
          precoPor: "R$0.00",
          description:
            "Abriremos para você como funciona a nossa estratégia vencedora de investimentos.",
        },
        {
          img: "/img/bonus2.jpg",
          titulo: "Acesso à metodologia X-green",
          precoDe: "R$1.599",
          precoPor: "R$0.00",
          description:
            "Abriremos para você como funciona a nossa estratégia vencedora de investimentos.",
        },
        {
          img: "/img/bonus3.jpg",
          titulo: "Acesso à metodologia X-green",
          precoDe: "R$1.599",
          precoPor: "R$0.00",
          description:
            "Abriremos para você como funciona a nossa estratégia vencedora de investimentos.",
        },
        {
          img: "/img/bonus4.jpg",
          titulo: "Acesso à metodologia X-green",
          precoDe: "R$1.599",
          precoPor: "R$0.00",
          description:
            "Abriremos para você como funciona a nossa estratégia vencedora de investimentos.",
        },
        {
          img: "/img/bonus5.jpg",
          titulo: "Acesso à metodologia X-green",
          precoDe: "R$1.599",
          precoPor: "R$0.00",
          description:
            "Abriremos para você como funciona a nossa estratégia vencedora de investimentos.",
        },
        {
          img: "/img/bonus6.jpg",
          titulo: "Acesso à metodologia X-green",
          precoDe: "R$1.599",
          precoPor: "R$0.00",
          description:
            "Abriremos para você como funciona a nossa estratégia vencedora de investimentos.",
        },
        {
          img: "/img/bonus7.jpg",
          titulo: "Acesso à metodologia X-green",
          precoDe: "R$1.599",
          precoPor: "R$0.00",
          description:
            "Abriremos para você como funciona a nossa estratégia vencedora de investimentos.",
        },
        {
          img: "/img/bonus8.jpg",
          titulo: "Acesso à metodologia X-green",
          precoDe: "R$1.599",
          precoPor: "R$0.00",
          description:
            "Abriremos para você como funciona a nossa estratégia vencedora de investimentos.",
        },
      ],
      items: [
        { text: "Real-Time", icon: "mdi-clock" },
        { text: "Audience", icon: "mdi-account" },
        { text: "Conversions", icon: "mdi-flag" },
      ],

      listItems1: [
        { desc: "Curso completo" },
        { desc: "Acesso às entradas" },
        { desc: "Grupo Vip no Telegram" },
        { desc: "Planilha de gestão de bancas" },
        { desc: "Acesso a novos mercados" },
        { desc: "Consultoria Six Capital" },
        { desc: "8 bônus exclusivos" },
        { desc: "Suporte on-line" },
      ],
    };
  },
};
</script>


<style scoped lang="scss">
@media(max-width: 991px) {
  .wrapper {
    padding: 70px 20px !important;
  }
}
.wrapper {
  background: #111111;
  padding: 100px;
  text-align: center;
}

.title-bonus {
  width: 100%;
  max-width: 500px;
  h2 {
    color: #a6ff3f;
    font-size: 4rem;
    text-transform: uppercase;
  }
  p {
    color: #ffffff;
    font-size: 1.2rem;
  }
}

/* ================ 8 Cards ========================== */

.container-bonus {
  min-width: 200px;
  min-height: 300px;
  max-width: 200px;
  max-height: 300px;
  border: 8px solid #606060;
  border-radius: 4px;
  display: flex;
  align-items: center;
  h2 {
    color: #ffffff;
  }
}
.p-desc {
  text-align: initial;
  color: #ffffff;
  max-width: 200px;
}
.container-p {
  display: flex;
  .p-green {
    color: chartreuse;
    text-decoration: line-through;
  }
  .p-red {
    color: crimson;
  }
}

.btn-pers{
  border-radius: 30px;
  margin-top: -25px;
  width: 220px;
}

/* ========================== */

/* ==============Container pink & green ==================== */
.container-adesao {
  width: 100%;
  max-width: 900px;
  margin: 0 auto;
}
.c-text-div {
  width: 100%;
}
.border-green {
  width: 100%;
  height: 160px;
  border-top: 4px solid #a6ff3f;
  border-left: 4px solid #a6ff3f;
  border-right: 4px solid #a6ff3f;
  border-top-left-radius: 20px;
  border-top-right-radius: 20px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;

  .h2-c-green {
    color: #a6ff3f;
    text-transform: uppercase;
  }
  .p-c-green {
    color: #ffffff;
  }
}
.background-pink {
  width: 100%;
  padding: 20px;
  background: #f71c43;
  border-bottom-left-radius: 20px;
  border-bottom-right-radius: 20px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  .text-bp {
    text-transform: uppercase;
    max-width: 680px;
    margin: 0 auto;
  }
  .text-white {
    color: #ffffff;
  }
  .text-black {
    color: #111111;
    font-weight: 600;
    white-space: nowrap;
  }
  .text-brackground {
    background-color: #ffffff;
  }
}

.btn-adesao {
  margin-top: -480px;
  height: 48px;
  width: 320px;
  border: none;
  border-radius: 20px;
  text-align: center;
  background-color: #ffffff;
  color: #f71c43;
  font-size: 18px;
  font-weight: 600;
  text-transform: uppercase;
  &:hover {
    background-color: #e9e3e3;
  }
}

@media (max-width: 900px) {
  .btn-adesao {
    width: 150px;
    height: 30px;
    font-size: 12px;
    margin-top: 4px;
  }
}
/* =========================== */

/* ===========Card adesão ================ */

.c-adesao {
  width: 260px;
  height: 460px;
}

.c-green {
  width: 100%;
  height: 12%;
  background: #a6ff3f;
  display: flex;
  justify-content: center;
  align-items: center;
  border-top-left-radius: 8px;
  border-top-right-radius: 8px;
  text-decoration: line-through;
}

.c-grey {
  width: 100%;
  height: 26%;
  background: #919191;
  display: flex;
  justify-content: center;
  align-items: flex-end;
  padding-bottom: 4px;
  .c-border {
    width: 80%;
    height: 70%;
    border: 3px solid;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
  }
  .h2-mensal {
    background-color: #919191;
    position: relative;
    top: -8px;
  }
  .h1-green {
    color: #a6ff3f;
    font-size: 50px;
  }
}
.c-list-desc {
  background: #f2f2f2;
  width: 100%;
  height: 68%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding-left: 2px;
  border-bottom-left-radius: 8px;
  border-bottom-right-radius: 8px;
  li {
    list-style: none;
  }
  ul {
    padding-left: 0px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    font-size: 14px;
    padding-bottom: 30px;
    :first-child {
      color: #a6ff3f;
      font-size: 12px;
      text-transform: uppercase;
      font-weight: bold;
    }
  }
}

button {
  width: 80%;
  background: #a6ff3f;
  color: #ffffff;
  height: 14%;
  border-radius: 6px;
  text-transform: uppercase;
  font-weight: bold;
}
</style>
