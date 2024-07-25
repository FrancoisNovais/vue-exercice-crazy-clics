<script setup>
function getRandomInt(max) {
  return Math.floor(Math.random() * max)
}

const displayRandomNumber = () => {
  alert(getRandomInt(99))
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
  border: none;
  border-style: double;
  color: white;
  padding: 65px 20px;
  font-size: 16px;
  border-radius: 50%;
}
</style>
