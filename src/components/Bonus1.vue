<script setup>
const word1 = 'aLigaTOR'
const word2 = 'CHAMOIS'
const word3 = 'ElEpHaNt'
const word4 = 'wombaT'

const correctTheWord = (word) => {
  let str = ''
  for (let i = 0; i < word.length; i++) {
    if (i === 0) {
      str = str + word[i].toUpperCase()
    } else {
      str = str + word[i].toLowerCase()
    }
  }
  alert(str)
}
</script>

<template>
  <section>
    <button @:click="correctTheWord(word1)">{{ word1 }}</button>
    <button @:click="correctTheWord(word2)">{{ word2 }}</button>
    <button @:click="correctTheWord(word3)">{{ word3 }}</button>
    <button @:click="correctTheWord(word4)">{{ word4 }}</button>
  </section>
</template>

<style scoped>
section {
  justify-content: center;
  gap: 30px;
}
button {
  background-color: #62e5b3;
  padding: 7px 15px;
  border: none;
  border-radius: 5px;
}
</style>
