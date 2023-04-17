<template>
  <HeaderApp title="Yu-Gi-Ho" />
  <div>

  </div>
</template>

<script>
import { store } from './store';
import axios from 'axios';
import HeaderApp from './HeaderApp.vue';
  export default {
    name: 'App',

    components : {
      HeaderApp,
    }
    
  }
</script>

<style lang="scss" scoped>

</style>