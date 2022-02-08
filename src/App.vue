<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from './components/HelloWorld.vue'
import Calculatrice from './components/Calculatrice.vue';
import Convertisseur from './components/Convertisseur.vue';
import Inscription from './components/Inscription.vue';
</script>

<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <Inscription></Inscription>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
