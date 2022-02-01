<template>
    <!-- v-on:click is same as @click -->
    <button v-on:click="onClick()" :style="{background: color}" class="btn">{{text}}</button>
</template>

<script>
export default {
    name: "Button",
    props: {
        text: String,
        color: String    
    },
    methods: {
        onClick(){
            this.$emit("btn-click")
        }
    }
}


</script>