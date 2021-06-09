<template>
  <section class="wrapper">
    <v-container>
      <div class="title-bonus mx-auto mb-15">
        <h2
          :class="
            $vuetify.breakpoint.smAndUp ? '' : 'display-1 font-weight-bold'
          "
        >
          Bônus!
        </h2>
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
              <div style="background-color: #00ff00" class="rounded-lg color-indice mb-2"></div>
              <h2 class="title lh-125">
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
            <div class="c-text-div px-3 py-5">
              <div class="h2-c-green text-uppercase">
                <div
                  :class="
                    $vuetify.breakpoint.smAndUp ? 'display-1' : 'headline'
                  "
                  class="font-weight-bold"
                >
                  São mais de R$ 7 mil em bônus,
                </div>
                <div
                  :class="
                    $vuetify.breakpoint.smAndUp ? 'headline' : 'subtitle-1'
                  "
                  class="font-weight-medium"
                >
                  + acesso à metodologia exclusiva fast green<sup class="body-2">&reg;</sup>
                </div>
              </div>
              <div class="p-c-green pt-1 text-lg-h5 text-sm-body-2 text-uppercase">
                E você não vai pagar por nenhum deles!
              </div>
            </div>
          </div>
          <div class="background-pink pb-12 pt-10">
            <div class="c-text-div">
              <div
                :class="$vuetify.breakpoint.smAndUp ? 'headline' : ''"
                class="text-lg-h5 text-bp"
              >
                <span class="text-white">E vamos além,</span>
                <span class="text-black"> vamos te dar R$ 3.000,00<br>de desconto no curso </span>
                <b class="text-brackground px-2">Até dia 25/04</b>
              </div>
            </div>
          </div>
          <v-btn x-large color="white" class="pink--text btn-pers">
            <span class="title font-weight-black">+ Adesão zero</span>
          </v-btn>
        </div>
      </v-container>
      <!-- ========================================================= -->
      <!-- <section class="container-cards"> -->
      <div
        class="d-flex justify-center mb-10 mt-10 white--text"
        :class="$vuetify.breakpoint.smAndUp ? 'headline' : 'subtitle-1'"
      >
        Começando hoje, você vai ter:
      </div>
      <v-row class="d-flex align-center">
        <v-col cols="12" sm="12" md="6" lg="4" class="c-adesao ma-auto mb-10">
          <div class="c-green">
            <h4>Adesão: R$ 399</h4>
          </div>
          <div class="c-grey">
            <h2 class="h2-mensal">Mensal</h2>
            <div class="c-border">
              <div class="c-b-h1">
                <h1 class="h1-green">299,</h1>
              </div>
              <div class="c-b-p">
                <p>00</p>
                <p class="pl-2">p/mês</p>
              </div>
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
        </v-col>

        <v-col cols="12" sm="12" md="6" lg="4" class="ma-auto mb-7 mx-adesao">
          <div class="c-green white">
            <h4>Adesão: R$ 399</h4>
            <img
              class="img-desconto"
              src="/img/selo_85desconto.png"
              alt="Bonus 85% de desconto"
            />
          </div>
          <div class="c-grey verde-escuro">
            <h2 class="h2-mensal verde-escuro">Anual</h2>
            <div class="c-border">
              <div class="c-b-h1">
                <h1 class="h1-green white--text">49,</h1>
              </div>
              <div class="c-b-p">
                <p class="white--text">00</p>
                <p class="pl-2">p/mês</p>
              </div>
            </div>
          </div>
          <div class="c-list-desc verde-claro">
            <ul class="desc-card">
              <li v-for="(listItem1, i) in listItems1" :key="i">
                <v-icon small color="grey darken-2"> mdi-check-bold </v-icon>
                {{ listItem1.desc }}
              </li>
            </ul>

            <button class="pink white--text">Quero começar</button>
          </div>
        </v-col>
        <v-col cols="12" sm="12" md="6" lg="4" class="c-adesao ma-auto mb-10">
          <div class="c-green active">
            <h4>Adesão: R$ 399</h4>
          </div>
          <div class="c-grey">
            <h2 class="h2-mensal">Semestral</h2>
            <div class="c-border">
              <div class="c-b-h1">
                <h1 class="h1-green">199,</h1>
              </div>
              <div class="c-b-p">
                <p>00</p>
                <p class="pl-2">p/mês</p>
              </div>
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
        </v-col>
      </v-row>
      <div
        class="d-flex justify-center mb-10 mt-10 white--text"
        :class="$vuetify.breakpoint.smAndUp ? 'body-1' : 'body-2'"
      >
        Formas de pagamento: Cartão de Crédito,  2 Cartões de Crédito, PIX, Boleto Bancário, Débito Bancário, Cartão de débito virtual Caixa, Conta Hotmart, PayPal, GooglePay e SamsungPay
      </div>
      <div class="d-flex justify-center">
        <img src="/img/logos_pagamentos.jpg" alt="" />
      </div>
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
          titulo: "Acesso à metodologia X-Green",
          precoDe: "Imensurável!",
          precoPor: "R$0.00",
          description:
            "Conheça detalhadamente a estratégia vencedora da X-Green",
        },
        {
          img: "/img/bonus2.jpg",
          titulo: "Acesso ao Grupo Vip Telegram X-Green",
          precoDe: "R$300",
          precoPor: "R$0.00",
          description:
            "No grupo, você poderá copiar as nossas entradas e lucrar mais",
        },
        {
          img: "/img/bonus3.jpg",
          titulo: "Acesso às planilhas vencedoras X-Green",
          precoDe: "R$200",
          precoPor: "R$0.00",
          description:
            "Gestão de banca, juros compostos e evolução dos resultados",
        },
        {
          img: "/img/bonus4.jpg",
          titulo: "Consultoria de planejamento financeiro e investimentos Six Capital",
          precoDe: "R$5.000",
          precoPor: "R$0.00",
          description:
            "Aprenda com uma das melhores consultorias do mercado",
        },
        {
          img: "/img/bonus5.jpg",
          titulo: "Guia: como não ser limitado nas casas",
          precoDe: "R$500",
          precoPor: "R$0.00",
          description:
            "As casas de investimentos não impedirão o seu crescimento",
        },
        {
          img: "/img/bonus6.jpg",
          titulo: "Como fazer o seu IR ",
          precoDe: "R$200",
          precoPor: "R$0.00",
          description:
            "Aprenda a declarar os seus lucros",
        },
        {
          img: "/img/bonus7.jpg",
          titulo: "Investimentos em outros esportes",
          precoDe: "R$1.000",
          precoPor: "R$0.00",
          description:
            "Corridas de galgos e mais novidades",
        },
        {
          img: "/img/bonus8.jpg",
          titulo: "Lives exclusivas ",
          precoDe: "R$300",
          precoPor: "R$0.00",
          description:
            "Veja vídeos exclusivos com os nossos especialistas",
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
@media (max-width: 991px) {
  .wrapper {
    padding: 70px 20px !important;
  }
}
.wrapper {
  background: #111111;
  padding: 40px 100px;
  text-align: center;
}
.color-indice{
  height: 10px;
  width: 40px;
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
  align-items: flex-start;
  justify-content: flex-end;
  flex-direction: column;
  padding: 10px;
  h2 {
    color: #ffffff;
    text-align: initial;
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

.btn-pers {
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

.img-desconto {
  position: relative;
  bottom: -20px;
  right: -20px;
  width: 100px;
  height: 100px;
}

.c-adesao {
  max-width: 290px;
  height: 460px;
}
.mx-adesao {
  max-width: 300px;
  height: 480px;
  ul {
    :first-child {
      color: #000000 !important;
    }
  }
  .c-green {
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }
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
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding-bottom: 4px;
  .c-border {
    width: 80%;
    border: 3px solid;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 10px;
  }
  .h2-mensal {
    background-color: #919191;
    position: relative;
    bottom: -20px;
  }
  .c-b-h1 {
    width: 60%;
    .h1-green {
      display: flex;
      justify-content: flex-end;
      align-items: center;
      color: #a6ff3f;
      font-size: 50px;
    }
  }
  .c-b-p {
    width: 40%;
    max-height: 200px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;

    :first-child {
      color: #a6ff3f;
      font-size: 25px;
      font-weight: bold;
    }
    p {
      margin: 0;
      padding: 0;
    }
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
    padding-left: 0;
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
  background: #7fd12d;
  color: #ffffff;
  height: 14%;
  border-radius: 6px;
  text-transform: uppercase;
  font-weight: bold;
}

.verde-claro{
  background: #a6fe3e;
}
.verde-escuro{
  background-color: #7fd12d !important;
}
.lh-125{
  line-height: 1.25;
}
</style>
