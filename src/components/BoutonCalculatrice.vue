<template>
    <div><button v-for="element in elements" :keys="element" @click="sendValue(element)"><span class="d-flex">{{ element }}</span></button></div>
</template>

<script>
import { defineComponent } from "@vue/runtime-core";


export default defineComponent(
    {
        data(){
            return{
                elements: ["1","2",'3',"4","5","6","7","8","9","+","-","/","*"],
            }
        },
        emits: ["update-data"],
        methods:
        {
            sendValue(data)
            {
                this.$emit("update-data",data);
            }
        }
    }
)

</script>