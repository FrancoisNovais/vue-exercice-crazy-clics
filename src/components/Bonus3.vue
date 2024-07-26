<script setup>
const colorsList = [
  { name: 'bleu', hexa: '#0B71BA' },
  { name: 'vert', hexa: '#39B639' },
  { name: 'orange', hexa: '#EA8512' },
  { name: 'violet', hexa: '#721D7D' },
  { name: 'marron', hexa: '#713928' },
  { name: 'jaune', hexa: '#DED94B' },
  { name: 'noir', hexa: '#1C1C18' },
  { name: 'rouge', hexa: '#F11919' },
  { name: 'gris', hexa: '#9C9696' }
]

const randomColorBis = () => {
  const randomIndex = Math.floor(Math.random() * colorsList.length)
  alert(
    `Vous obtenez du ${colorsList[randomIndex].name} dont le code hexadécimal est ${colorsList[randomIndex].hexa} .`
  )
}
</script>

<template>
  <section>
    <div>
      <button @:click="randomColorBis(getRandomInt)">Couleur surprise version bis</button>
    </div>
  </section>
</template>

<style scoped>
section {
  justify-content: center;
}
div {
  background: linear-gradient(90deg, red, orange, yellow, green, blue);
}
button {
  background: white;
  padding: 7px 20px;
  font-weight: bold;
  margin: 2px;
  border: none;
}
</style>
