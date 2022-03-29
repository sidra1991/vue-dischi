<template>
  <header>
    <ricerca-pazza/>
  </header>
</template>

<script>
import ricercaPazza from './ricercaPazza.vue'

export default {
  components: { ricercaPazza },
  name: 'HelloWorld'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  background-color: #2e3a46;
  height: 10vh;
}
</style>
