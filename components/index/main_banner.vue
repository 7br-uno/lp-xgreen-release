<template>
  <div class="banner">
    <header>
      <a href="#" class="logo">
        <img src="/img/logo_home.png" alt="" />
      </a>
    </header>
    <img class="img-bg" src="/img/bg_home.jpg" alt="">
    <div class="content">
      <p>Tenha ganhos</p>
      <h2>Realmente assustadores</h2>
    </div>
  </div>
</template>
<style scoped lang="scss">

@media(max-width: 991px) {
  .banner {
    padding: 50px !important;
    header {
      padding: 20px 50px !important;
    }
    .content{
      h2 {
        font-size: 36px !important;
      }
      p {
        font-size: 16px !important;
      }
    }
  }
  .logo {
    img {
      width: 60px;
      height: 25px;
    }
  }
}

.banner {
  position: relative;
  width: 100%;
  height: 100vh;

  display: flex;
  justify-content: center;
  align-items: center;
  .img-bg{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  .content {
    position: relative;
    max-width: 750px;
    p {
      color: #fff;
      font-size: 18px;
      text-transform: uppercase;
    }
    h2 {
      color: #a7e853;
      font-size: 60px;
      text-transform: uppercase;
      line-height: 1.2;
      filter: drop-shadow(-1px -1px 7px #a7e853);
    }
  }
  header {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    padding: 40px 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 10000;
  }
}
</style>
