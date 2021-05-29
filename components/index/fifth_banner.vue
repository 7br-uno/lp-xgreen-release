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
  padding: 6.25rem;
  .container{
    padding: 0 15.625rem 0 15.625rem;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    flex-direction: column;
    h2 {
      font-size: 2.5rem;
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
      height: 2.5rem;
      border-radius: 1.25rem;
      padding-top: 1.25rem;
      margin: 1.25rem 0 1.25rem 0;

      p{
        text-transform: uppercase;
        font-weight: 600;
      }
    }
  }
}

@media screen and (max-width: 1080px){
  html {
    font-size: 93.75%;
  }
}

@media screen and(max-width: 720px){
  html {
    font-size: 87.5%;
  }
}

@media screen and(max-width: 600px){
  html {
    font-size: 75%;
  }
}
</style>
