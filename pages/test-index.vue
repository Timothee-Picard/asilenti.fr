<template>
  <div>
    <input type="text" v-model="value" />
    <p>Value: {{ value }}</p>
    <p>{{el}}</p>
  </div>
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

<style scoped>

</style>
