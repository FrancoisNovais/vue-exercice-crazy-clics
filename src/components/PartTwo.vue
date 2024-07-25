<script setup>
const displayName = () => {
  console.log("Je m'appelle François")
}
const displayName2 = () => {
  alert("Je m'appelle François")
}
</script>

<template>
  <div>
    <button @click="displayName">Comment t'appeles-tu</button>
    <button @:click="displayName2">Comment t'appeles-tu</button>
  </div>
</template>

<style scoped></style>
