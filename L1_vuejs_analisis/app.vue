<!--Implementación de un componente básico-->
<template>
  <div>
    <!--{{ nombre }} muestra el dato-->
    <h1>Holi {{ nombre }}</h1> 
    <!-- v-model="nombre" permite editarlo desde el imput-->
    <input v-model="nombre" placeholder="Editar nombre" />
    <p>Contador: {{ contador }}</p>
    <button @click="incrementar">Incrementar</button>
  </div>
</template>

<script>
// data es el MODEL, el template es la VIEW, y methods es VIEWMODEL, es decir, la lógica que conecta el modelo con la vista.
export default {
  data() {
    return {
      nombre: "Jimena",
      contador: 0
    };
  },
  methods: {
    incrementar() {
      this.contador++;
    }
  }
};
</script>

<style>
h1 {
  color: #a78bfa; /* tono pastel */
}
</style>