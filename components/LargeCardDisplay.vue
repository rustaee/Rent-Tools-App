<template>
  <b-container class="large-card-display">
    <b-row>
      <b-col>
        <h1>{{ cardInfo.title }}</h1>
        <p>{{ cardInfo.snippet }}</p>
        <b-card-group deck>
          <SingleCard
          v-for="card in cardInfo.cards"
          :key="card.id"
          :info="card"
         />
        </b-card-group>
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
.card-deck{
  align-items: stretch;
}

.large-card-display{
  margin-bottom: 30px;
}
h1{
  font-size: 1.2rem;
}
</style>