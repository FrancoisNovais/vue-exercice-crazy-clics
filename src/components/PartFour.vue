<script setup>
function getRandomInt(max) {
  return Math.floor(Math.random() * max)
}

const displayRandomNumber = () => {
  alert(getRandomInt(100))
}
</script>

<template>
  <section>
    <button @:click="displayRandomNumber">Chiffre surprise</button>
  </section>
</template>

<style scoped>
section {
  justify-content: center;
}
button {
  background-color: #fc7440;
  border: double rgb(237, 218, 151);
  color: white;
  width: 160px;
  height: 160px;
  font-size: 16px;
  border-radius: 50%;
}
</style>
