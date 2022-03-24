<template>
  <main>
    <CardsCompositions/>
  </main>
</template>

<script>
import CardsCompositions from './CardsCompositions.vue'
export default {
  name: 'MainContainerColor',
  components: {
    CardsCompositions
  }
}
</script>

<style scoped lang="scss">
 main{
  height: 95vh;
  background-color: #1e2d3b ;
  display: flex;
  align-items: center;
  justify-content: center;
 }

</style>
