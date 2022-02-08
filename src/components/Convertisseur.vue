<template>
    <p>en Km</p>
    <input v-model="value" />
    <p>en M</p>
    <p>{{ KmToM }}</p>
    <p>en Cm</p>
    <p>{{ KmToCm }}</p>
    <p>en mm</p>
    <p>{{ KmToMm }}</p>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
    data() {
        return {
            value: null,
        };
    },
    computed:
    {
        KmToM() {
            return this.value * 1000;
        },
        KmToCm() {
            return this.value * 10000;
        },
        KmToMm() {
            return this.value * 100000;
        }
    },
    method:
    {
    }
})
</script>
