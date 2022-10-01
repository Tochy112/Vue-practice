<template>
    <div>
        <button :style="{backgroundColor: color}">{{text}}</button>
    </div>
</template>

<script>
    export default{
        name: "Button",

        props: {
            text: String,
            color: String
        },

       
    }
</script>

<style scoped>
    button{
        padding: 10px;
        border-radius: 5px;
        background-color: #000;
        color: #fff;
        font-size: large;
        cursor: pointer;
        max-width: max-content;
    }
</style>