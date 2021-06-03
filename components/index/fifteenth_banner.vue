<template>
  <v-footer color="black" class="white--text py-16">
    <v-container class="my-16">
      <v-row>
        <v-col cols="12" md="6">
          <div class="d-flex align-center">
            <div class="mx-auto ml-sm-0">
              <img src="/img/logo_xgreen_rodape.png" alt="X-GREEN" />
              <p>Siga as nossas redes sociais</p>
              <a class="pr-5" href="#">
                <img src="/img/logo_facebook.png" alt="logo-facebook"/>
              </a>
              <a href="#">
                <img src="/img/logo_instagram.png" alt="logo-instagram"/>
              </a>
              <a class="pl-5" href="#">
                <img src="/img/logo_twitter.png" alt="logo-twitter" />
              </a>
            </div>

          </div>
        </v-col>
        <v-col cols="12" md="6">
          <div class="caption">
            <p>
              Resultados passados não são garantias de resultados futuros. As
              informações deste site destinam-se ao seu conhecimento geral e não
              garantimos resultados especificos e valores exatos de lucro. Os
              resultados são de inteira responsibilidade do assinante e/ou aluno que
              realiza suas próprias operações.
            </p>
            <p>
              O nosso conteúdo tem fins de conhecimento e cultura. São voltados à
              introdução aos conhecimentos em educação e mercados financeiros, dentro
              dos melhores valores éticos e morais, com o objetivo de promover as
              habilidades necessárias para o correto entendimento eme educação
              financeira.
            </p>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-footer>
</template>
<style scoped lang="scss">
.footer {
  background: #000000;
  display: flex;
  justify-content: space-between;
  align-items: center;

  .logo-icones{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    img {
      padding-bottom: 2rem;
    }
    p{
      color: #ffffff;
      text-transform: uppercase;
    }
    ul {
      width: 100%;
      display: flex;
      flex-direction: row;
      justify-content: flex-start;
      padding-left: 0 !important;
    }
    li {
      list-style: none;
      img {
        margin-right: 1rem;
      }
    }

  }

  .descriptions{
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    p {
      color: #ffffff;
      font-size: 0.6rem;
    }
  }

}
</style>
