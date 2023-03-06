<script>
export default {
  data(){
    return { 
      contador: 10
  }
  },
  methods:{
    incrementar(){
      this.contador++
    },
    decrementar (){
      if (this.contador > 0) {
        this.contador--
      }
    },
    reset(){
      this.contador = 0
    }
  }
}
</script>

<template>
  <button @click="incrementar">+</button>
  <button @click="decrementar">-</button>
  <button @click="reset">c</button>
  <p>Valor do contador: {{  contador }}</p>
</template>

<style scoped>
button {
  margin-left: 10px;
  background-color: brown;
  color: black;
  border: none;
  border-radius: 5px;
  padding: 5px 10px;
  cursor: pointer;  
}</style>
