<template>
   <div>
      <exchangele-nav-bar :brandName="brandName" :menuItems="menuItems" />
      <exchangele-hero/>
      <exchangele-list/>
      <exchangele-pagination/>
  </div>
</template>


<script>
  import ExchangeleNavBar from '@/components/NavBar.vue'
  import ExchangeleHero from '@/components/Hero.vue'
  import ExchangeleList from './components/ExchangeleList.vue'
  import ExchangelePagination from './components/Pagination.vue'
export default {
  name: 'App',
  components:{
    ExchangeleNavBar,
    ExchangeleHero,
    ExchangeleList,
    ExchangelePagination
  },
      data() {
          return {
            brandName: "Exchagario",
            menuItems:[
              {text: "HOME", link:"/" },
              {text: "ABOUT", link:"/about"},
              {text: "FAQ", link:"/faq" },
              {text: "LOGIN", link:"/login" },
              {text: "REGISTER", link:"/register" },
            ]
          }
        }
}
</script>

<style lang="scss">
    @import './assets/styles/variables.scss';
    @import '~bulma/bulma.sass';
    @import './assets/styles/main.scss'; 
</style>