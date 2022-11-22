<template>
  <section class="section-create">
    <img src="~assets/img/page-home/line-create.svg" class="bg-line">
    <aside>
      <div class="content">
        <h2>Créez votre site internet</h2>
        <p>Lorem Ipsum, giving information on its origins, as well as a random Lipsum generator.</p>
        <button>Découvrir</button>
      </div>
    </aside>
    <main>
      <ul>
        <li>
          <b>1</b>
          <p>Lorem Ipsum, giving information on its origins, as well as a random Lipsum generator.</p>
        </li>
        <li>
          <b>2</b>
          <p>Lorem Ipsum, giving information on its origins, as well as a random Lipsum generator.</p>
        </li>
        <li>
          <b>3</b>
          <p>Lorem Ipsum, giving information on its origins, as well as a random Lipsum generator.</p>
        </li>
        <li>
          <b>4</b>
          <p>Lorem Ipsum, giving information on its origins, as well as a random Lipsum generator.</p>
        </li>
        <li>
          <b>5</b>
          <p>Lorem Ipsum, giving information on its origins, as well as a random Lipsum generator.</p>
        </li>
      </ul>
    </main>
  </section>
</template>

<script setup>

</script>

<style lang="scss" scoped>
section {
  padding-top: 15em;
  padding-bottom: 5em;
  display: flex;
  position: relative;
  .bg-line {
    width: 80%;
    position: absolute;
    top: 5em;
    left: -30%;
  }
  main, aside {
    flex: 1;
    display: flex;
  }
  aside {
    display: flex;
    justify-content: center;
    position: sticky;
    top: 50%;
    transform: translateY(-50%);
    height: fit-content;
    margin-top: 200px;
    .content {
      max-width: 453px;
    }
  }
  main {
    display: flex;
    ul {
      list-style: none;
      display: flex;
      justify-content: space-between;
      flex-direction: column;
      max-width: 450px;
      margin-left: 5em;
      gap: 5em;
      li {
        display: flex;
        padding: 100px 0 100px 3em;
        border-left: 3px solid transparent;
        color: #8A8D94;
        &:hover {
          border-left: 3px solid #CF525E;
          b {
            color: #CF525E;
          }
        }
        b {
          width: 110px;
          font: normal normal normal 90px/75px Catellos;
        }
      }
    }
  }
}
</style>
