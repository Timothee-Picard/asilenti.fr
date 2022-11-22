<template>
  <HomeSectionDevelop />
  <HomeSectionCreate />
  <section class="section-offers">
    AAAAAA
    <input type="checkbox" name="" id="">
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
.section-offers {
  position: relative;
  background-color: #080912;
  border-radius: 85px 85px 0px 0px;
  margin-top: 250px;
  &:before {
    content: '';
    position: absolute;
    width: 400px;
    height: 400px;
    background: url("~/assets/img/page-home/top-stains-offers.svg") no-repeat center;
    background-size: contain;
    top: -256px;
    left: 50%;
    transform: translateX(-50%);
  }
  input {
    appearance: none;
  }
}
</style>
