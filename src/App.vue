<template>
    <!-- <RouterLink to="/" class="button">Notes</RouterLink>  -->
    <!-- <RouterLink to="/stats" class="button">Stats</RouterLink> -->
    <NavBar/>
    <div class="container is-max-desktop px-2 py-4">
        <RouterView/>
    </div>
   
</template>

<script setup>
import NavBar from './components/Layout/NavBar.vue';
</script>

<style>
@import 'bulma/css/bulma.min.css'
</style>