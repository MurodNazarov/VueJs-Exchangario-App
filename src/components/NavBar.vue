<template>
     <header class="header">
      <nav class="navbar">
        <div class="container">
          <div class="navbar-brand">
            <a class="navbar-item has-text-white is-size-2 has-text-weight-bold" href="#">
              {{brandName}}
            </a>
            <span role="button" tabindex="0" class="navbar-burger burger has-text-white" data-target="navbar-menu">
              <span></span>
              <span></span>
              <span></span>
            </span>
          </div>
          <div id="navbar-menu" class="navbar-menu">
            <div class="navbar-end">
              <!-- Loop through the navigation items -->
              <a 
              v-for="item in menuItems"
              :key="item.text"
              class="navbar-item nav-home" :href="item.link">{{item.text}}</a>
             
            </div>
          </div>
        </div>
      </nav>
    </header>
</template>

<script>
    export default {
        props:{
          brandName:{
            type: String
          },
          menuItems:{
            type: Array,
            require: true
          }
        }
    }
</script>

<style lang="scss" scoped>

</style>