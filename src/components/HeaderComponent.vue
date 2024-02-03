<template>
  <header>
    <div class="logo">
      <a href="/">
        <img src="../assets/logo.svg" />
      </a>
    </div>
    <button class="btn btn-lang">ru</button>
  </header>
</template>

<script>
export default {
  name: "HeaderComponenet,",
};
</script>

<style scoped lang="scss">
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-top: 40px;

  @media (max-width: 900px) {
    padding-top: 20px;
  }

  .logo img {
    width: 100%;

    @media (max-width: 900px) {
      width: calc(180px + (250 - 180) * ((100vw - 375px) / (900 - 375)));
    }
  }
}
.btn-lang {
  width: 50px;
  height: 50px;
  border-radius: 100%;
  background: #29d1a9;
  font-size: 16px;
  box-shadow: 0 4px 4px 0 rgba(0, 0, 0, 0.25);

  @media (max-width: 900px) {
    width: 40px;
    height: 40px;
    font-size: 14px;
  }
}
</style>
