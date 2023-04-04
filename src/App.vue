<script>
  const numero = 10;
  export default{
    data:() => ({
      contador: 10
    }),
    methods:{
      saludar(){
        console.log("hola")
      },
      sumar(){
        this.contador++
      },
      restar(){
        this.contador--
      },
      reset(){
        this.contador = 0
      }
    },
    //data(){
      //return{
        //contador: 200
      //}
    //}
  }
</script>

<template>
  <div class="container">
    <small>
      <h1>Aprendiendo VUE</h1>
    </small>
    <img src="./assets/logo.svg" alt="Logo VUE" width="125" height="125">
    <hr>
    <h2>Contador: {{ contador }}</h2>
    <button v-on:click="sumar()">+1</button>
    <button @click="restar()">-1</button>
    <button @click="reset()">Reset</button>
  </div>
</template>

<style scoped> 
  small{
    color: green;
  }
  h1{
    font-size: 2.5rem;
    font-weight: bolder;
  }
  h2{
    font-size: 1.5rem;
  }
  button{
    cursor: pointer;
    font-size: 1rem;
    margin: 0px 6px;
  }
  .container{
    text-align: center;
    background-color: whitesmoke;
  }
</style>
