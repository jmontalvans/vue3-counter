<script>
  export default {
    data:()=>({
      contador:10,
    }),
    methods:{
      incrementar(){
        this.contador++
      },
      disminuir(){
        this.contador--
      },
      reset(){
        this.contador = 10
      }
    }
  }
</script>

<template>
  <img src="./assets/logo.svg" alt="" height="120" width="120">
  <h1>Hola mundo de Vue</h1>
  <hr />

  <h2>Contador: {{ contador }}</h2>
  <button @click="incrementar()">+1</button>
  <button @click="disminuir()">-1</button>
  <button @click="reset()">Reset</button>


</template>