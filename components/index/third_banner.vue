<template>
  <section class="wrapper">
    <div class="container">
      <h2>Para quem é este curso ?</h2>
      <ul
        v-for="benefit in benefits"
        :key="benefit"
      >
        <li>
          <img :src="benefit.img" :alt="benefit.text">
          <p> {{benefit.text}}</p>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data: () => {
    return {
      benefits:[
        {img: "/img/icone_paraquemcurso_01.png", text: "Para quem deseja lucrar com investimento esportivo"},
        {img: "/img/icone_paraquemcurso_02.png", text: "Quer completar a sua renda ou aprender uma nova profissão"},
        {img: "/img/icone_paraquemcurso_03.png", text: "Quem busca a liberdade financeira a médio e longo prazo"},
        {img: "/img/icone_paraquemcurso_04.png", text: "Quem precisa de uma acessoria de investimentos esportivo que lucra em mais de 95% dos dias"},
        {img: "/img/icone_paraquemcurso_05.png", text: "Para quem já investe e quer diversificar a carteira"},
      ]
    }
  }
}
</script>
<style scoped lang="scss">
.wrapper {
  width: 100%;
  background: #2A2A2A;
  padding: 100px;
  display: flex;
  justify-content: center;
  .container {
    width: 50%;
    padding: 0 2rem;
    border: 3px solid #ffff;
    h2{
      text-align: center;
      position: relative;
      top: -20px;
      background-color: #2A2A2A;
      color: #ffff;
      font-weight: 600;
      font-size: 30px;
      text-transform: uppercase;
      line-height: 1;
    }
    ul{
      display: flex;
      justify-content: end;
      align-items: center;
      li{
        list-style: none;
        display: flex;
        padding-bottom: 2rem;
        align-items: center;
        img{
          margin-right: 2rem;
          max-width: 50px;
        }
        p{
          color: #ffff;
          padding-top: 0.5rem;
        }
      }
    }
  }
}
</style>
