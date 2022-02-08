<template>
    <div v-if="!validation">
        <label for="name">Votre nom : </label>
        <input type="text" v-model="nom" />
        <br>
        <label for="prenom">Votre prénom : </label>
        <input type="text" v-model="prenom" />
        <br />
        <label for="date">Votre date de naissance : </label>
        <input type="text" v-model="date" />
        <br />
        <label for="date">Votre adresse mail : </label>
        <input type="text" v-model="adresse" />
        <br />
        <button @click="validation = true">Valider</button>
    </div>
    <div v-if="validation">Félicitations, vous êtes inscrits.</div>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
    data() { 
        return {
        nom: null,
        prenom: null,
        date: null,
        adresse: null,
        validation: false,
    };},
})
</script>
