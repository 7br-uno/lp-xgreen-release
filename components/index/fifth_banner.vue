<template>
  <section class="wrapper">
    <div class="container">
      <h2>Você acha que está muito bom para ser verdade?</h2>
      <div class="container-attention">
        <p>Então preste atenção</p>
      </div>
      <p>
        Desde 2018, a X-green conseguiu
        <b>
          lucro em mais de 95% dos dias.
        </b>
      </p>
      <p>
        <b>
          É isso mesmo! Finalizamos mais de 95% de todos os dias com lucro desde 2018.
        </b>
      </p>
    </div>
  </section>
</template>
<style scoped lang="scss">
.wrapper {
  width: 100%;
  background: #fffd00;
  padding: 100px;
  .container{
    padding: 0px 250px 0px 250px;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    flex-direction: column;
    h2 {
      font-size: 40px;
      text-transform: uppercase;
      line-height: 1;
      font-weight: 600;
    }
    p {
      line-height: 0.5;
    }
    .container-attention {
      width: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #ffff;
      height: 40px;
      border-radius: 20px;
      padding-top: 20px;
      margin: 20px 0px 20px 0px;

      p{
        text-transform: uppercase;
        font-weight: 600;
      }
    }
  }
}
</style>
