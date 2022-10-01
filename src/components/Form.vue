<template>
    <form>
        <div>
            <label for="username">Username</label>
            <input type="text" v-model="username" placeholder="Enter your username" name="username">
            {{username}}
        </div>
        <div>
            <label for="password">Password</label>
            <input type="password" v-model="password" placeholder="Enter your full name" name="password">
        </div>

        <Button text="Submit" />
    </form>
</template>

<script>
    import Button from "./Button"

    export default {
        name: "Form",

        components: {
            Button
        },

        data(){
            return {
                username: "",
                password: ""
            }
        }
    }
</script>

<style scoped>
    form div{
        display: flex;
        flex-direction: column;
        margin:10px;
    }
    form input{
        width: 80%;
        padding: 10px;
    }
  
    
</style>