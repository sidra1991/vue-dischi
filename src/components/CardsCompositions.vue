<template>
  <div class="center" >
    <div v-for="(links,index) in this.arrCards" :key="index" class="cards" >
      <img :src="links.poster" alt="">
      <h3>{{links.title}}</h3>
      <h4>{{links.author}}</h4>
      <h5>{{links.year}}</h5>
    </div>
  </div>
</template>

<script>
import axios from 'axios'

export default {
  name: 'CardsCompositions',
  data () {
    return {
      arrCards: null
    }
  },
  created () {
    axios.get('https://flynn.boolean.careers/exercises/api/array/music')
      .then((response) => {
        this.arrCards = response.data.response
        // console.log('primo -------', response)
        console.log('secondo -------', response.data)
      })
  }
}

</script>

<style>
  .cards {
    background-color: #2e3a46;
    height: 225px;
    width: 150px;
    display: flex;
    flex-wrap: nowrap;
    flex-direction: column;
    align-items: center;
    margin: 0.5rem;
  }

  img{
    margin-top: 10px;
    width: 100px;
  }

  h3{
    margin-top: 10px;
    color: white;
  }

  h4,h5{
    margin-top: 5px;
    color:#6b6e72;
  }

   .center {
   width: 80%;
   height: 90%;
   display: flex;
   flex-wrap: wrap;
  }

</style>
