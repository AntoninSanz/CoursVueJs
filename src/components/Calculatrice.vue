<template>
    <EcranCalculatrice />
    <BoutonCalculatrice @update-data="recupereDonnee" />
    <div>{{ valeur1 }}</div>
</template>
    
<script>
import { defineComponent } from "@vue/runtime-core";
import BoutonCalculatrice from "./BoutonCalculatrice.vue";
import EcranCalculatrice from "./EcranCalculatrice.vue";


export default defineComponent
(
    {
    data() {
        return {
            calculette: null,
            valeur1: null,
            valeur2: null,
            operateur: null
        };
    },
    components: { EcranCalculatrice, BoutonCalculatrice },
    methods: 
    {
        recupereDonnee(data)
        {
            console.log(data)
            if(this.valeur1 == null)
            {
                this.valeur1 = data;
            }
            else if(this.operateur == null)
            {
                this.operateur = data;
            }
            else
            {
                this.valeur2 = data;
            }
        }
    }
}
)
</script>