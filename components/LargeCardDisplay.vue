<template>
  <b-container>
    <b-row>
      <b-col>
        <h1>{{ cardInfo.title }}</h1>
        <p>{{ cardInfo.snippet }}</p>
        
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
h1{
  font-size: 1.2rem;
}
</style>