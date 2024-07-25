<script setup>
const convertToCm = (km) => {
  alert(`${km} km correspond à ${km * 100000} cm.`)
}
</script>

<template>
  <h2>Convertir des km en cm :</h2>
  <div>
    <button @click="convertToCm('10')">10 km</button>
    <button @click="convertToCm('50')">50 km</button>
    <button @click="convertToCm('145')">145 km</button>
    <button @click="convertToCm('459')">459 km</button>
    <button @click="convertToCm('1579')">1579 km</button>
    <button @click="convertToCm('3979')">3979 km</button>
    <button @click="convertToCm('5000')">5000 km</button>
    <button @click="convertToCm('7846')">7846 km</button>
    <button @click="convertToCm('10979')">10979 km</button>
  </div>
</template>

<style scoped>
button {
  padding: 25px 65px;
  text-align: center;
  font-size: 16px;
}
</style>
