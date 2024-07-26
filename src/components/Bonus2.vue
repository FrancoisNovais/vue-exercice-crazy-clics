<script setup>
const colorsList = [
  'bleu',
  'vert',
  'rose',
  'orange',
  'violet',
  'marron',
  'jaune',
  'noir',
  'rouge',
  'gris'
]

const randomColor = () => {
  const randomIndex = Math.floor(Math.random() * colorsList.length)
  alert(colorsList[randomIndex])
}
</script>

<template>
  <section>
    <button @:click="randomColor">Couleur surprise</button>
  </section>
</template>

<style scoped>
section {
  justify-content: center;
}
button {
  background: none;
  padding: 7px 15px;
  font-weight: bold;
  border-radius: 20px;
  color: #6f146f;
  border: 2px solid#6f146f;
}
</style>
