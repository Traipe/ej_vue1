<!--Single File Component-->
<template>
  <!--Acá va el html-->
  <main id="app">
    <h1>Hola Vue ✌️</h1>
    <h2>Contador: {{ contador }}</h2>
    <button @click="saludar">Aumentar ➕</button>
  </main>
</template>

<script>
// acá va la lógica de nuestro componente
export default {
  name: 'App',
  //Lo que haya dentro de data seran variables reactivas, es decir, que si cambian su valor, se va a actualizar la vista  
  data() {
    return {
      contador: 0
    }
  },
  methods: {
    saludar() {
      this.contador++;
    }
  }
}
</script>

