<script setup>
import { RouterLink, RouterView } from 'vue-router'
import NavBar from "./components/NavBar.vue"


</script>

<template>
 <NavBar class="navbar" />
  <RouterView />
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: rbga(59,59,59);
}
</style>
