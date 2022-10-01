<template>
  <div class="container">
    <Header content="Hello World" />
    <Form />
  </div>
</template>


<script>
  import Header from "./components/Header"
  import Form from "./components/Form"

  export default {
    name : "App",

    components : {
      Header,
      Form
    }
  }
</script>

<style scoped>
  .container{
    display: flex;
    flex-direction: column;
    border: 1px solid blue;
    border-radius: 5px;
    width: 400px;
    min-height: 300px;
    margin: 30px auto ;
  }
</style>