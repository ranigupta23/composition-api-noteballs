<template>
    <nav class="navbar has-background-primary" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <div class="navbar-item is-size-4 is-family-monospace">
        Noteballs
     </div>


    <a role="button" @click.prevent="showMobileNav=!showMobileNav" class="navbar-burger" :class="{'is-active':showMobileNav}" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>

  <div id="navbarBasicExample" class="navbar-menu" :class="{'is-active':showMobileNav}">
    <div class="navbar-end">
        <RouterLink to="/" class="navbar-item" active-class="is-active">
        Notes 
      </RouterLink>

      <RouterLink to="/stats" class="navbar-item" active-class="is-active">
        Stats
      </RouterLink>
      
    </div>
  </div>
</nav>
</template>

<script setup>
import {ref} from 'vue'
const showMobileNav=ref(true)
</script>

<style>
@media (max-width:1023px){
    .navbar-menu{
        position:absolute;
        left:0;
        width:100%;
    }
}
</style>