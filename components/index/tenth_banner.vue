<template>
  <section class="wrapper">
    <div class="title-bonus mx-auto mb-15">
      <h2>Bônus!</h2>
      <p>
        E garantindo a sua vaga no
        <b>período promocional você ganha mais 8 bônus:</b>
      </p>
    </div>
    <v-row>
      <v-col cols="12" sm="6" md="3" v-for="cardBonus in cardsBonus" :key="cardBonus.titulo">
        <span class="text-xl-h4 text-sm-body-2">TESTE</span>
      </v-col>
    </v-row>
    <div class="container-cards-bonus">
      <ul class="list-cards">
        <li v-for="cardBonus in cardsBonus" :key="cardBonus.titulo">
          <div
            class="container-bonus"
            :style="`background: url(${cardBonus.img}); background-size: cover; background-position: center`"
          >
            <span></span>
            <h2>
              {{ cardBonus.titulo }}
            </h2>
          </div>
          <div class="container-p">
            <p class="p-green">{{ cardBonus.precoDe }} |</p>
            <p class="p-red">
              {{ cardBonus.precoPor }}
            </p>
          </div>
          <p>
            {{ cardBonus.description }}
          </p>
        </li>
      </ul>
    </div>
    <div class="container-adesao">
      <div class="border-green">
        <h2>
          São mais de R$ 7 mil em bônus + acesso à metodologia exclusiva fast
          green
        </h2>
        <p>E você não vai pagar por nenhum deles!</p>
      </div>
      <div class="background-pink">
        <h2>
          <span class="text-white">E vamos além,</span> vamos te dar
          <span class="text-black">R$ 3.000,00</span> de desconto no curso
          <b class="text-brackground">Até dia 25/04</b>
        </h2>
      </div>
    </div>
    <button class="btn-adesao">+ Adesão zero</button>
    <!-- ========================================================= -->
    <section class="container-cards">
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
            <li  v-for="(listItem1, i) in listItems1" :key="i">
              <v-icon small color="grey darken-2">
                mdi-check-bold
              </v-icon>
              {{listItem1.desc}}
            </li>
          </ul>

           <button>Quero começar</button>

        </div>
      </div>
    </section>
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
        {desc: "Curso completo"},
        {desc: "Acesso às entradas"},
        {desc: "Grupo Vip no Telegram"},
        {desc: "Planilha de gestão de bancas"},
        {desc: "Acesso a novos mercados"},
        {desc: "Consultoria Six Capital"},
        {desc: "8 bônus exclusivos"},
        {desc: "Suporte on-line"},
      ],
    };
  },
};
</script>


<style scoped lang="scss">
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

.container-cards-bonus {
  width: 100%;
  display: flex;
  .list-cards {
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    li {
      margin-left: 0 !important;
      width: 25%;
      height: 40rem;
      list-style: none;
      height: x;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      p {
        text-align: initial;
        color: #ffffff;
      }
      .container-p {
        display: flex;
        .p-green {
          color: chartreuse;
        }
        .p-red {
          color: crimson;
        }
      }
      .container-bonus {
        width: 80%;
        height: 50%;
        border: 8px solid #606060;
        border-radius: 4px;
        display: flex;
        align-items: center;
        h2 {
          color: #ffffff;
        }
      }
    }
  }
}

.container-adesao {
  width: 100%;
}

.border-green {
  width: 100%;
  height: 10rem;
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
  h2 {
    color: #a6ff3f;
    font-size: 1.6rem;
    text-transform: uppercase;
    padding: 0rem 20rem 0 20rem;
  }
  p {
    color: #ffffff;
    font-size: 1.2rem;
  }
}
.background-pink {
  width: 100%;
  height: 10rem;
  background: #f71c43;
  border-bottom-left-radius: 20px;
  border-bottom-right-radius: 20px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  h2 {
    font-size: 1.6rem;
    text-transform: uppercase;
    padding: 0rem 20rem 0 20rem;
    font-weight: 400;
  }
  .text-white {
    color: #ffffff;
  }
  .text-black {
    color: #111111;
    font-weight: 600;
  }
  .text-brackground {
    background-color: #ffffff;
  }
}

.btn-adesao {
  margin-top: -30rem;
  height: 3rem;
  width: 20rem;
  border: none;
  border-radius: 20px;
  text-align: center;
  background-color: #ffffff;
  color: #f71c43;
  font-size: 1.2rem;
  font-weight: 600;
  text-transform: uppercase;
  &:hover {
    background-color: #e9e3e3;
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
