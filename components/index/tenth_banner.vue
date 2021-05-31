<template>
  <section class="wrapper">
    <div class="title-bonus">
      <h2>Bônus!</h2>
      <p>E garantindo a sua vaga no <b>período promocional você ganha mais 8 bônus:</b></p>
    </div>
    <div class="container-cards-bonus">
      <ul class="list-cards">
        <li v-for="cardBonus in cardsBonus" :key="cardBonus">
          <div class="container-bonus" :style="`background: url(${cardBonus.img}); background-size: cover; background-position: center`">
            <span></span>
            <h2>
              {{cardBonus.titulo}}
            </h2>
          </div>
          <div class="container-p">
            <p class="p-green">
              {{cardBonus.precoDe}} |
            </p>
            <p class="p-red">
              {{cardBonus.precoPor}}
            </p>
          </div>
          <p>
            {{cardBonus.description}}
          </p>
        </li>
      </ul>
    </div>
    <div class="container-adesao">
      <div class="border-green">

      </div>
      <div class="background-pink">

      </div>
    </div>
  </section>
</template>

<script>

export default {
  data: () => {
    return {
      cardsBonus:[
        {img: "/img/bonus1.jpg", titulo: "Acesso à metodologia X-green", precoDe: "R$1.599", precoPor: "R$0.00", description: "Abriremos para você como funciona a nossa estratégia vencedora de investimentos."},
        {img: "/img/bonus2.jpg", titulo: "Acesso à metodologia X-green", precoDe: "R$1.599", precoPor: "R$0.00", description: "Abriremos para você como funciona a nossa estratégia vencedora de investimentos."},
        {img: "/img/bonus3.jpg", titulo: "Acesso à metodologia X-green", precoDe: "R$1.599", precoPor: "R$0.00", description: "Abriremos para você como funciona a nossa estratégia vencedora de investimentos."},
        {img: "/img/bonus4.jpg", titulo: "Acesso à metodologia X-green", precoDe: "R$1.599", precoPor: "R$0.00", description: "Abriremos para você como funciona a nossa estratégia vencedora de investimentos."},
        {img: "/img/bonus5.jpg", titulo: "Acesso à metodologia X-green", precoDe: "R$1.599", precoPor: "R$0.00", description: "Abriremos para você como funciona a nossa estratégia vencedora de investimentos."},
        {img: "/img/bonus6.jpg", titulo: "Acesso à metodologia X-green", precoDe: "R$1.599", precoPor: "R$0.00", description: "Abriremos para você como funciona a nossa estratégia vencedora de investimentos."},
        {img: "/img/bonus7.jpg", titulo: "Acesso à metodologia X-green", precoDe: "R$1.599", precoPor: "R$0.00", description: "Abriremos para você como funciona a nossa estratégia vencedora de investimentos."},
        {img: "/img/bonus8.jpg", titulo: "Acesso à metodologia X-green", precoDe: "R$1.599", precoPor: "R$0.00", description: "Abriremos para você como funciona a nossa estratégia vencedora de investimentos."},
      ]
    }
  }
}
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
    color: #A6FF3F;
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
      margin-left: 0!important;
      width: 25%;
      height: 40rem;
      list-style: none;
      height: x;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      p{
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

.container-adesao{
 width: 100%;
}

.border-green {
  width: 100%;
  height: 10rem;
  border-top: 4px solid #A6FF3F ;
  border-left: 4px solid #A6FF3F;
  border-right: 4px solid #A6FF3F;
  border-top-left-radius: 20px;
  border-top-right-radius: 20px;
}
.background-pink {
  width: 100%;
  height: 10rem;
  background:#F71C43;
  border-bottom-left-radius: 20px;
  border-bottom-right-radius: 20px;
}

</style>
