<script setup>
import PartOne from './components/PartOne.vue'
import PartTwo from './components/PartTwo.vue'
import PartThree from './components/PartThree.vue'
import PartFour from './components/PartFour.vue'
import PartFive from './components/PartFive.vue'
import PartSix from './components/PartSix.vue'
</script>
<template>
  <main>
    <h1>Crazy clics</h1>
    <PartOne />
    <PartTwo />
    <PartThree />
    <PartFour />
    <PartFive />
    <PartSix />
  </main>
</template>

<style scoped>
main {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
