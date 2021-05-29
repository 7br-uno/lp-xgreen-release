<template>
  <section class="wrapper">
    <h2>E mais: Temos o Robozão absurdamente bom!</h2>
    <p class="text-green">(E que não foi barato)</p>
    <div class="container">
      <div class="robozao_strategist">
        <div>
          <img src="/img/icone_robozao_televisao_01.png" alt="" />
          <p>
            Uma inteligência artificial, apelidada de Robozão, indicada as
            nelhores entradas e jogos da nossa estratégia vencedora desde 2018
          </p>
        </div>
      </div>
      <div class="robozao_strategist">
        <div>
          <img src="/img/icone_robozao_uniao_02.png" alt="" />
          <p>
            Uma inteligência artificial, apelidada de Robozão, indicada as
            nelhores entradas e jogos da nossa estratégia vencedora desde 2018
          </p>
        </div>
      </div>
      <div class="robozao_strategist">
        <div>
          <img src="/img/icone_robozao_bola_03.png" alt="" />
          <p>
            Uma inteligência artificial, apelidada de Robozão, indicada as
            nelhores entradas e jogos da nossa estratégia vencedora desde 2018
          </p>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped lang="scss">
.wrapper {
  background: #191919;
  padding: 50px;
  text-align: center;
  h2 {
    color: #ffff;
    font-size: 2.5rem;
    text-transform: uppercase;
    line-height: 1;
    padding: 0 15.625rem 0 15.625rem;
  }
  .text-green {
    color: #a7e853;
    font-size: 18px;
    text-transform: uppercase;
    line-height: 2;
    padding: 0 15.625rem 0 15.625rem;
  }
  .container {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    margin-top: 60px;

    .robozao_strategist {
      position: relative;
      width: 350px;
      height: 400px;
      display: flex;
      justify-content: center;
      align-items: center;
      img {
        max-width: 100px;
        padding-bottom: 1rem;
      }
      p {
        font-size: 1rem;
        text-align: initial;
        color: #ffff;
      }
    }
  }
}
</style>
