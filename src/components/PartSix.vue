<script setup>
const displayNetwork = (network) => {
  alert(`Il s'agit du réseaux  ${network}`)
}
</script>

<template>
  <div>
    <font-awesome-icon @click="displayNetwork('Github')" :icon="['fab', 'github']" />
    <font-awesome-icon @click="displayNetwork('LinkedIn')" :icon="['fab', 'linkedin']" />
    <font-awesome-icon @click="displayNetwork('Instagram')" :icon="['fab', 'instagram']" />
  </div>
</template>

<style scoped>
svg {
  font-size: 48px;
  padding: 10px;
}
</style>
