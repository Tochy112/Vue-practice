<template>
    <div class="header">
        <h1>{{content}}</h1>
        <Button text="Click Me" color="green"/>
        <Button @click="click" text="Sign In" color="blue"/>
    </div>
</template>

<script>
    import Button from "./Button"

    export default{
        name: "Header",

        props: {
            content: String,
        },

        components: {
            Button
        },

        methods: {
            click(){
                prompt("Enter your username") ? alert("logged in succesfully") : ""
            }
        }


    }
</script>

<style scoped>
    .header{
        display: flex;
        justify-content: space-evenly;
        align-items: center;
    }
</style>