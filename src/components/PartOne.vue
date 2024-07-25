<script setup>
const handleClick = () => {
  console.log('Hello world !')
}
const handleClickTwo = () => {
  console.log('Bienvenue au Reacteur !')
}
</script>

<template>
  <section>
    <button v-on:click="handleClick">Affiche un message dans la console</button>
    <button @:click="handleClickTwo">Affiche un autre message dans la console</button>
  </section>
</template>

<style scoped>
section {
  justify-content: center;
  gap: 40px;
}
button {
  padding: 8px;
  color: #daa521;
  border: 2px #daa521 solid;
  background-color: white;
  border-radius: 8px;
}
</style>
