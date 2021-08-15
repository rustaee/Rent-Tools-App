<template>
  <b-container class="large-card-display">
    <b-row>
      <b-col>
        <h2>{{ cardInfo.title }}</h2>
        <b-row cols="4" class="bg-dark p-4" no-gutters>
          <SingleSmallCard
          v-for="card in cardInfo.cards"
          :key="card.id"
          :info="card"
         />
        </b-row>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  props: ['cardInfo']
}
</script>

<style lang="scss" scoped>
.large-card-display{
  margin-bottom: 30px;
}
h2{
  font-size: 1.1rem;
}
</style>