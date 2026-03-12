<!--Reutilización y modularidad-->
<template>
  <div class="tarjeta">
    <h2>{{ nombre }}</h2>
    <p>Contador: {{ contador }}</p>
    <button @click="$emit('reset')">Resetear</button>
  </div>
</template>

<script>
export default {
  props: {
    nombre: String,
    contador: Number
  }
};
</script>

<style>
.tarjeta {
  border: 1px solid #d1d5db;
  padding: 1rem;
  border-radius: 8px;
  background-color: #f3f4f6;
}
</style>

<!-- La arquitectura basada en componentes permite reutilizar código, mantenerlo modular y facilitar la escalabilidad-->
 