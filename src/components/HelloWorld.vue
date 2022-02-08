<template>
  <input type="text" v-model="result" />
  <span v-if="result === 'coucou'">{{ result }}</span>
  <ul>
    <li v-for="legume in legumes" :key="legume">{{ legume }}</li>
  </ul>
  <span @click="counter++">{{ counter }}</span>
  <v-card>
    <v-alert type="primary" :value="true">
    ça fonctionne
  </v-alert>
  </v-card>
  <v-btn color="success" class="d-flex justify-center">text</v-btn>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>

<script>

import { defineComponent } from 'vue';


export default defineComponent({
  data() {
    return {
      result: "",
      legumes: ["courgette", "carott", "cucurbitacé"],
      counter: 0,
    }
  },
})
</script>