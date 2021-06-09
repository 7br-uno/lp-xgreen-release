<template>
  <section class="wrapper">
    <v-container class="px-0 px-md-16">
      <h1 class="text-center mb-6">Perguntas frequentes</h1>
      <v-expansion-panels
        multiple
        v-for="(question, i) in questions"
        :key="i"
        class="px-lg-16"
      >
        <v-expansion-panel class="bg-panel">
          <v-expansion-panel-header class="panel-title"
            >{{ question.title }}
          </v-expansion-panel-header>
          <v-expansion-panel-content class="panel-description">
            {{ question.description }}
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-container>
  </section>
</template>

<script>
export default {
  data: () => {
    return {
      questions: [
        {
          title: "Como funciona o teste de 7 dias / cancelamento",
          description: "Ao optar pelo teste grátis, você terá até 7 dias para cancelar a sua inscrição na plataforma de compra, sem enrolação.",
        },
        {
          title: "O Ambiente de pagamento é seguro?",
          description: "A plataforma Hotmart certifica a segurança e a proteção de seus dados pessoais e financeiros.",
        },
        {
          title: "Quais são as formas de pagamento?",
          description: "Trabalhamos com as seguintes formas de pagamento: Cartão de Crédito,  2 Cartões de Crédito, PIX, Boleto Bancário, Débito Bancário, Cartão de débito virtual Caixa, Conta Hotmart, PayPal, GooglePay e SamsungPay.",
        },
        {
          title: "Preciso entender de futebol?",
          description: "Não, para iniciar no método da X-Green não é preciso entender de futebol ou de outros esportes. Nós ensinamos tudo de uma maneira fácil, do básico ao avançado.",
        },
        {
          title: "Preciso ter muito dinheiro?",
          description: "Não, durante o curso você vai aprender técnicas para começar a investir com pouco dinheiro.",
        },
        {
          title: "Como acesso o Grupo Vip?",
          description: "Ao realizar a sua compra, será disponibilizado um link de acesso exclusivo para o Grupo Vip, onde você poderá copiar as nossas entradas.",
        },
        {
          title: "Como funciona o suporte?",
          description: "Nossa equipe está sempre ligada. Mande um e-mail ou WhatsApp que responderemos quaisquer dúvidas.",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.wrapper {
  background: #000000;
  padding: 30px 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  h1 {
    color: #ffffff;
    padding-bottom: 1rem;
    text-transform: uppercase;
    font-size: 3rem;
  }
}
.bg-panel {
  background-color: #292828 !important;
  margin-bottom: 1rem;
}
.panel-title {
  font-weight: 600;
  text-transform: uppercase;
  color: #ffffff;
}


.panel-description {
  color: #ffffff;
}
</style>
