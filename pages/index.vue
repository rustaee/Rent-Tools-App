<template>
  <b-container fluid="md">
    <Hero />
    <LargeCardDisplay v-for="card in largeCards" :key="card.id" :cardInfo="card"/>
  </b-container>
</template>

<script>
import { largeCardSections } from '@/assets/data.js'
export default {
  data(){
    return{
      largeCards: largeCardSections,
    }
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Righteous&display=swap');

h1, h2, h3, h4, .font-righteous{
  font-family: 'Righteous', cursive;
}

</style>
