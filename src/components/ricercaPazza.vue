<template>
  <form>
    <input type="text">
    <button type="button" :click="$emit()" ></button>
    <!-- <button type="button" :click="decerca()" ></button> -->
  </form>
</template>

<script>

export default {
  name: 'ricercaPazza'
}
</script>

<style>

</style>
