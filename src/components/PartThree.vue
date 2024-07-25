<script setup>
const colors = {
  bleue: '#23b8d3',
  violette: '#a519a5',
  orange: '#ffa500',
  verte: '#44f178'
}
const displayColor = (colorName) => {
  alert(`Il s'agit de la couleur ${colorName} dont le code hexadécimal est '${colors[colorName]}'.`)
}
</script>

<template>
  <h2>De quelle couleur s'agit-il ?</h2>
  <div class="color-list">
    <div @click="displayColor('bleue')" class="blueBg"></div>
    <div @click="displayColor('violette')" class="purpleBg"></div>
    <div @click="displayColor('orange')" class="orangeBg"></div>
    <div @click="displayColor('verte')" class="greenBg"></div>
  </div>
</template>

<style scoped>
.color-list {
}
.color-list div {
  height: 100px;
  width: 100px;
  border-radius: 60px 5px 60px 5px;
}
.blueBg {
  background-color: #23b8d3;
}
.purpleBg {
  background-color: #a519a5;
}
.orangeBg {
  background-color: #ffa500;
}
.greenBg {
  background-color: #44f178;
}
</style>
