<template>  
  <div class="body-container">
    <navbar />
    <b-container fluid="lg">
      <LargeCardDisplay v-for="card in largeCards.slice(0, 1)" :key="card.id" :cardInfo="card"/>
      <SmallCardDisplay v-for="card in smallCards" :key="card.id" :cardInfo="card"/>
    </b-container>
  </div>
</template>

<script>
import { largeCardSections } from '@/assets/data.js'
import { smallCardSections } from '@/assets/data.js'
import Navbar from '@/components/Navbar.vue'
export default {
  components: { Navbar },
  data(){
    return{
      largeCards: largeCardSections,
      smallCards: smallCardSections
    }
  }
}
</script>

<style lang="scss" scoped>

</style>