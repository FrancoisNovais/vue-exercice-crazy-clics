<script setup>
const displayName = () => {
  console.log("Je m'appelle François")
}
const displayName2 = (name) => {
  alert(`Je m'appelle ${name}`)
}
</script>

<template>
  <section>
    <button @click="displayName">Comment t'appeles-tu</button>
    <button @:click="displayName2('François')">Comment t'appeles-tu</button>
  </section>
</template>

<style scoped>
section {
  justify-content: space-around;
}
button {
  padding: 10px;
  color: white;
  border: none;
  background-color: white;
  border-radius: 20px;
  background: linear-gradient(to top right, #a7e2e2, #8a82c9);
}
</style>
