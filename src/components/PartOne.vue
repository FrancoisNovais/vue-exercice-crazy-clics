<script setup>
const handleClick = () => {
  console.log('Hello world !')
}
const handleClickTwo = () => {
  console.log('Bienvenue au Reacteur !')
}
</script>

<template>
  <div>
    <button v-on:click="handleClick">Affiche un message dans la console</button>
    <button @:click="handleClickTwo">Affiche un autre message dans la console</button>
  </div>
</template>

<style scoped></style>
