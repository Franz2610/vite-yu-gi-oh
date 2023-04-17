<template>
  <HeaderApp title="Yu-Gi-Oh API" />
  <MainCard/>
</template>

<script>
import { store } from './store';
import axios from 'axios';
import HeaderApp from './HeaderApp.vue';
import MainCard from './MainCard.vue';
  export default {
    name: 'App',

    components : {
      HeaderApp,
      MainCard
    },
    data(){
      return{
        store
      }
    },
    methods: {
      getCard(){
        const url = store.url
        axios.get(url).then((res) =>{
          store.cardList = res.data.results;
        });
      }
    },
    mounted() {
      this.getCard();
    }
    
  }
</script>

<style lang="scss" scoped>

</style>