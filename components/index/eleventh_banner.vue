<template>
  <div class="wrapper py-16">
    <v-container>
      <v-row>
        <v-col cols="12" offset-sm="5" sm="6" class="px-8 px-sm-0">
          <div class="teste-gratis">
            <h2 :class="$vuetify.breakpoint.smAndUp ? 'display-1' : 'headline'" class="font-weight-bold white--text mb-5">Sua experiência vai ser matadora!!!</h2>
            <p>Então <b>teste o nosso produto gratis por sete dias.</b>
              Aproveite este periodo e confirme o nosso rendimento e tudo o que estamos afirmando aqui!
            </p>
            <p>Se não quiser continuar, cancelamos a sua inscrição sem qualquer enrolação.</p>
            <p>É só entrar na plataforma de contratação do curso e solicitar o cancelamento.</p>

            <button>Faça o teste grátis por 7 dias</button>
          </div>
        </v-col>
        <v-col class="d-none d-md-block" sm="1">
          <img style="margin-left: -80%; margin-top: -80%;" src="/img/selo_setedias.png" alt="sete dias">
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<style scoped lang="scss">
.wrapper {
  background: url('/img/bg_jason.jpg');
  background-size: cover;
  background-position: center;
  background-repeat:no-repeat;
  .teste-sete {
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
