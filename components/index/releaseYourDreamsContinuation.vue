<template>
  <section class="wrapper">
    <h2 class="text-title">Tudo que você vê no mercado em um curso só</h2>
    <div class="courses-container">
      <div class="courses-container-cards">
        <div class="card-md">
          <h2>Aprenda de um jeito fácil.</h2>
          <p>Do basico ao avancçado:</p>
        </div>
        <button>Comece agora</button>
      </div>
      <ul class="courses-container-cards">
        <li
        class="card"
          v-for="course1 in courses1"
          :key="course1"
        >
          <p>{{ course1 }}</p>
        </li>
      </ul>
      <ul class="courses-container-cards">
        <li
        class="card"
          v-for="course2 in courses2"
          :key="course2"
        >
          <p>{{ course2 }}</p>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data: () => {
    return {
      courses1: [
        "Cadastros e operações nas casas de investimentos",
        "Uso correto de calculadoras",
        "Controle emocional/ Gestão de banca",
        "Estratégias conservadoras e arrojadas",
      ],
      courses2: [
        "Investimentos em futebol e outras modalidades",
        "Planejamento financeiro/juros compostos",
        "Conceitos: ODDs, ROI, Punter, Trader, etc",
        "Grupo Vip do Telegram com entradas para copiar",
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.wrapper {
  background: #141414;
  text-align: center;
  width: 100%;
  .text-title{
    font-size: 40px;
    line-height: 1.2;
    color: #ffff;
    padding: 0 30rem 0rem 30rem;
    font-weight: 600;
  }
  .courses-container {
    width: 100%;
    display: flex;
    justify-content: center;
    li{
      list-style: none;
    }
  }
  .courses-container-cards {
    width: 33.33%;
    height: 600px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    .card {
      width: 70%;
      text-align: center;
      height: 16%;
      border-radius: 10px;
      background-color: #606060;
      padding: 6%;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      margin-bottom: 2%;
      p{
        color: #fff;
      }
    }
    .card-md {
      width: 60%;
      text-align: center;
      height: 50%;
      border-radius: 10px;
      background-color: #292828;
      padding: 4%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      margin-bottom: 2%;
      h2{
        color: #ffff;
        font-size: 2.0rem;
        text-transform: uppercase;
        text-align: initial;
      }
      p{
        color: #ffff;
        font-size: 1.0rem;
        text-transform: uppercase;
        text-align: initial;
      }
    }
    button {
    background: #F71C43;
    height: 15%;
    border: none;
    width: 60%;
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
}
</style>
