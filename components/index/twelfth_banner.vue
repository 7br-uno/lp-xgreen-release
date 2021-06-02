<template>
  <section class="wrapper">
    <h1>Perguntas frequentes</h1>
    <v-expansion-panels
      v-model="panel"
      multiple
      v-for="(question, i) in questions"
      :key="i"
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
  </section>
</template>

<script>
export default {
  data: () => {
    return {
      questions: [
        {
          title: "Como funciona o teste de 7 dias/cancelamento",
          description: "",
        },
        {
          title: "Como funciona o teste de 7 dias/cancelamento",
          description: "",
        },
        {
          title: "Como funciona o teste de 7 dias/cancelamento",
          description: "",
        },
        {
          title: "Como funciona o teste de 7 dias/cancelamento",
          description: "Se você seguir a nossa estratégia exatamente à risca",
        },
        {
          title: "Como funciona o teste de 7 dias/cancelamento",
          description: "",
        },
        {
          title: "Como funciona o teste de 7 dias/cancelamento",
          description: "",
        },
        {
          title: "Como funciona o teste de 7 dias/cancelamento",
          description: "",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.wrapper {
  background: #000000;
  padding: 100px;
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
