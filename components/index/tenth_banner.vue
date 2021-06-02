<template>
  <section class="wrapper">
    <div class="title-bonus">
      <h2>Bônus!</h2>
      <p>
        E garantindo a sua vaga no
        <b>período promocional você ganha mais 8 bônus:</b>
      </p>
    </div>
    <div class="container-cards-bonus">
      <ul class="list-cards">
        <li v-for="cardBonus in cardsBonus" :key="cardBonus">
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
    <section class="container-card-adesao">
      <div class="adesao-green">
        <h4>Adesão: R$ 399</h4>
      </div>
      <div class="container-card-grey">
        <div class="container-border">
            <div>
             <h2 class="h2-mensal">Mensal</h2>
              <h1>299,</h1>
            </div>
            <div>
            <h2>00</h2>
            </div>
          </div>
         </div>
      <div>
        <ul>
          <li>Curso completo</li>
          <li>Curso completo</li>
          <li>Curso completo</li>
          <li>Curso completo</li>
          <li>Curso completo</li>
          <li>Curso completo</li>
          <li>Curso completo</li>
          <li>Curso completo</li>
          <li>Curso completo</li>
        </ul>
      </div>
      <div>
        <button>Quero começar</button>
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
  margin-bottom: 4rem;
  padding: 0 25rem;
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

.container-card-adesao{
  width: 250px;
  height: 400px;
  background: #f3f3f3;
  border-radius: 6px;
}

.adesao-green {
  width: 100%;
  height: 12%;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: #a6ff3f;

}

.container-card-grey{
  width: 100%;
  height: 40%;
  background: #919191;
  display: flex;
  justify-content: center;
  align-items: center;
}
.container-border {
  width: 80%;
  height: 80%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  border: solid 3px;
  margin-top: 1rem;

  .h2-mensal{
      background-color: #919191;
  }
    h1 {
      color: #a6ff3f;
      font-size: 4rem;
      font-weight: 600;
    }
}



</style>
