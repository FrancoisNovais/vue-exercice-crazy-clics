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
  <section>
    <h2>De quelle couleur s'agit-il ?</h2>
    <div class="color-list">
      <div @click="displayColor('bleue')" class="blueBg"></div>
      <div @click="displayColor('violette')" class="purpleBg"></div>
      <!-- With dynamic style inline -->
      <div @click="displayColor('orange')" :style="{ backgroundColor: colors.orange }"></div>
      <div @click="displayColor('verte')" :style="{ backgroundColor: colors.verte }"></div>
    </div>
  </section>
</template>

<style scoped>
section {
  flex-direction: column;
  align-items: center;
}

.color-list {
  display: flex;
  flex-direction: row;
  gap: 20px;
}
.color-list div {
  height: 80px;
  width: 80px;
  border-radius: 50px 5px 50px 5px;
}
.blueBg {
  background-color: #23b8d3;
}
.purpleBg {
  background-color: #a519a5;
}
</style>
