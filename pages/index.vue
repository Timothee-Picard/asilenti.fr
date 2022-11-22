<template>
  <HomeSectionDevelop />
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
  <section>
    AAAAAA
  </section>
  <section>
    AAAAAA
  </section>
</template>

<script setup>
import { ref, onMounted } from 'vue'
import { onUnmounted } from 'vue'

const value = ref('')
let el = ref('Miaou')
let intervalId

onMounted(() => {
  let i =0
  setInterval(function () {
    // console.log(el)
    el.value = "aaaaa"
  }, 1000);
})

onUnmounted(() => clearInterval(intervalId))
</script>

<style lang="scss">
section {
  min-height: 100vh;
}
h2 {
  font: normal normal normal 90px/85px Catellos;
  font-weight: 500;
}
.section-create {
  padding-top: 15em;
  padding-bottom: 20px;
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
    justify-content: center;
    position: sticky;
    top: 20px;
    height: fit-content;
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
      li {
        display: flex;
        padding: 50px 0 50px 3em;
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
