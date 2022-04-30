<template>
  <div>
      <nav-bar/>
      <Hero/>
      <exchangele-list/>
      <pagination/>
  </div>
</template>

<script>
  import NavBar from '@/components/NavBar.vue'
  import Hero from '@/components/Hero.vue'
import ExchangeleList from './components/ExchangeleList.vue'
import Pagination from './components/Pagination.vue'
export default {
  name: 'App',
  components:{
    NavBar,
    Hero,
    ExchangeleList,
    Pagination
  }
}
</script>

<style lang="scss">
    @import './assets/styles/variables.scss';
    @import '~bulma/bulma.sass';
    @import './assets/styles/main.scss'; 
</style>