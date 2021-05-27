<template>
  <div class="banner">
    <header>
      <a href="#" class="logo">Xgreen</a>
    </header>
    <div class="content">
      <p>Tenha ganhos</p>
      <h2>Realmente assustadores</h2>
    </div>
  </div>
</template>
<style scoped lang="scss">
.banner {
  position: relative;
  width: 100%;
  height: 100vh;
  background: #0a233f;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  padding: 200px;
  .content {
    position: relative;
    max-width: 750px;
    p {
      color: #fff;
      font-size: 18px;
      text-transform: uppercase;
      line-height: 0.5;
    }
    h2 {
      color: #a7e853;
      font-size: 50px;
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
    .logo {
      text-decoration: none;
      font-size: 24px;
      text-transform: uppercase;
      font-weight: 700;
      letter-spacing: 1px;
    }
  }
}
</style>
