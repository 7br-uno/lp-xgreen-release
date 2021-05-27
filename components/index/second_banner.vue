<template>
  <section class="wrapper">
    <div class="conatiner">
      <div class="column-left">
        <h1>Imagem</h1>
        <h2>Card</h2>
      </div>
      <div class="column-right">
        <p>Aqui você tem o </p>
        <h2>Curso mais completo</h2>
        <div class="card-p">
          <p>Assim como nós, transforme a sua vida!</p>
        </div>
        <div class="list-benefits">
          <ul>
            <li>
              <p>Ganhe uma renda extra todo mês</p>
            </li>
            <li>
              <p>Melhore de vida e de patamar financeiro</p>
            </li>
            <li>
              <p>Trabalhe de qualquer lugar. Basta um celular, internet e determinação</p>
            </li>
            <li>
              <p>Monte seu proprio horário. Bastam poucos minutos por dia</p>
            </li>
          </ul>
        </div>
        <Button>Comece agora</Button>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
  .wrapper {
    background: #131313;
    padding: 100px;
    text-align: center;
    .conatiner{
      width: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 80vh;
    }
  }
</style>
