<script setup>
const displayNetwork = (network) => {
  alert(`Il s'agit du réseaux  ${network}`)
}
</script>

<template>
  <section>
    <font-awesome-icon @click="displayNetwork('Github')" :icon="['fab', 'github']" />
    <font-awesome-icon @click="displayNetwork('LinkedIn')" :icon="['fab', 'linkedin']" />
    <font-awesome-icon @click="displayNetwork('Instagram')" :icon="['fab', 'instagram']" />
  </section>
</template>

<style scoped>
section {
  justify-content: center;
  gap: 30px;
}
svg {
  font-size: 48px;
}
</style>
