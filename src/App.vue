<template>
  <div class="bod">
    <HelloWorld/>
    <MainCardContainer/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MainCardContainer from './components/MainCardContainer.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    MainCardContainer
  }
}
</script>

<style lang="scss">
  *{
    margin: 0;
    box-sizing: border-box;
  }
</style>
