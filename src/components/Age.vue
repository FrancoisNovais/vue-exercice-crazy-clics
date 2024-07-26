<script setup>
import { ref } from 'vue'

const num = ref(0)

const decrease = () => {
  num.value--
}
const increment = () => {
  num.value++
}
const reset = () => {
  num.value = 0
}
</script>

<template>
  <section>
    <button @click="decrease">-</button><span>{{ num }}</span
    ><button @click="increment">+</button>
  </section>
  <button @click="reset">Reset counter</button>
</template>

<style scoped>
section {
  justify-content: center;
}
</style>
