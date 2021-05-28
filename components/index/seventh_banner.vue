<template>
  <section class="wrapper">
    <div class="f-container">
      <p class="first">Agora você pode estar pensando: como isso é possivel</p>
      <h2>Nós temos os melhores especialistas...</h2>
      <p class="second">Mas não nascemos prontos!</p>
    </div>
    <div class="s-container">
      <p>
        Operamos desde 2015. Fizemos <b>muitos</b> testes, erramos várias vezes,
        até chegar nesta estratégia <b>sólida e lucrativa</b>
      </p>
    </div>
  </section>
</template>
<style scoped lang="scss">
.wrapper {
  width: 100%;
  background: #131313;
  padding: 100px;
  display: flex;
  justify-content: center;
  align-items: flex-end;
  flex-direction: column;
  .f-container {
    width: 40%;
    padding: 50px;
    .first{
      color: #fff;
      font-size: 18px;
      text-transform: uppercase;

    }
    h2 {
      color: #a7e853;
      font-size: 50px;
      text-transform: uppercase;
      line-height: 1;
    }
    .second {
      color:  #a7e853;
      font-size: 18px;
      text-transform: uppercase;
    }
  }
  .s-container {
    width: 30%;
    padding: 20px 40px;
    display: flex;
    align-items: center;
    justify-content: center;
    p {
      color: #fff;
      font-size: 20px;
    }
  }
}
</style>
