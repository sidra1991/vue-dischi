<template>
  <div class="cards" >
    <img src="https://picsum.photos/200" alt="">
    <h2>bla bla</h2>
    <h3> bla lab </h3>
    <h4>1010</h4>
  </div>
</template>

<script>
export default {
  name: 'CardsCompositions'
}
</script>

<style>
  .cards {
    background-color: #2e3a46;
    height: 250px;
    width: 150px;
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
    align-items: center;
  }

  img{
    margin-top: 10px;
    width: 100px;
  }

  h2{
    margin-top: 10px;
    color: white;
  }

  h3,h4{
    margin-top: 5px;
    color:#6b6e72;
  }
</style>
