<template>
  <section>
    <main>
      <h2>Développer<br />votre <span>projet</span></h2>
      <form>
        <input type="text" name="" id="">
        <label>Déposer votre e-mail</label>
        <input type="submit" value="Envoyer">
      </form>
    </main>
    <aside>
      <img src="~/assets/img/page-home/line-arrow-project.svg" class="line-arrow">
      <p>
        Lorem Ipsum, giving information on its origins, as well as a random Lipsum generator.Lorem Ipsum, giving
        information on its origins, as well as a random Lipsum generator.
      </p>
      <div class="rs-icons">
        <i>IN</i>
        <i>F</i>
        <i>Y</i>
        <i>INS</i>
      </div>
    </aside>
    <img src="~/assets/img/page-home/stains-project.svg" class="corner-left">
  </section>
</template>

<script setup>

</script>

<style lang="scss" scoped>
section {
  display: flex;
  position: relative;
  main {
    flex: 1.2;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    h2 span {
      color: #CF525E;
    }
    form {
      margin-top: 18vh;
    }
  }
  aside {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: url("~/assets/img/page-home/bg_home-project.jpg") no-repeat center;
    background-size: cover;
    border-radius: 0px 0px 0px 26px;
    position: relative;
    overflow: hidden;
    p {
      max-width: 520px;
      color: white;
    }
    .line-arrow {
      width: 60%;
      position: absolute;
      top: 30%;
      transform: translateY(-50%);
      right: 60%;
    }
    .rs-icons {
      justify-self: flex-end;
    }
  }
  .corner-left {
    width: 60em;
    position: absolute;
    bottom: 0;
    transform: translateY(50%);
    left: -33em;
  }
}
</style>
