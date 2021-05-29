<template>
  <div class="banner">
    <header>
      <a href="#" class="logo">
        <img src="/img/logo_home.png" alt="" />
      </a>
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
  height: calc(100vh + 10rem);
  background: url("/img/bg_home.jpg");
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  padding: 12.5rem;
  .content {
    position: relative;
    max-width: 46.875rem;
    p {
      color: #fff;
      font-size: 1.125rem;
      text-transform: uppercase;
      line-height: 0.5rem;
    }
    h2 {
      color: #a7e853;
      font-size: 3.125rem;
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
    padding: 2.5rem 6.25rem;
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 10000;
  }
}
</style>
