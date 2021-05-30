<template>
  <section class="wrapper">
    <div class="teste-sete">
      <h2>Teste grátis</h2>
      <p>Ainda está achando que é muito bom pra ser verdade?</p>
      <div class="img-teste">
      <img src="/img/selo_setedias.png" alt="sete dias">
      </div>
    </div>
    <div class="teste-gratis">
      <p>Então <b>teste o nosso produto gratis por sete dias.</b>
      Aproveite este periodo e confirme o nosso rendimento e tudo o que estamos afirmando aqui!
      </p>
      <p>Se não quiser continuar, cancelamos a sua inscrição sem qualquer enrolação.</p>
      <p>É só entrar na plataforma de contratação do curso e solicitar o cancelamento.</p>

      <button>Faça o teste grátis por 7 dias</button>
    </div>
  </section>
</template>
<style scoped lang="scss">
.wrapper {
  background: url('/img/bg_jason.jpg');
  background-size: cover;
  background-position: center;
  background-repeat:no-repeat;
  padding: 100px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-direction: row;
  .teste-sete {
    width: 40%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    .img-teste {
      width: 100%;
      display: flex;
      justify-content: center;
    }

    h2{
      font-size: 2rem;
      text-transform: uppercase;
      color: #ffff;
      font-weight: 600;
      text-align: initial;
    }
    p{
      text-align: initial;
      color: #ffff;
    }

  }
  .teste-gratis{
    width: 40%;
    p{
      text-align: initial;
      color: #ffff;
    }
    button {
    margin-top: 2rem;
    width: 100%;
    background: #F71C43;
    height: 3rem;
    border: none;
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
