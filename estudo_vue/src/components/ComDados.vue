<template>
  <div>
    <h1>Componente com Dados</h1>
    <p>Nome: {{ nomeProduto }} - {{ codigoProduto }}</p>
  </div>
</template>

<style scoped>
div {
  text-align: center;
  border: 2px solid rgb(10, 69, 4);
  background-color: #050d04;
  margin: 30px;
  border-radius: 15px;
  padding: 10px;
}

p {
  font-size: 1.5rem;
}
</style>

<!-- <script>
//options API
export default {
  data: function () {
    return {
      nomeProduto: "Caderno",
      codigoProduto: "#321",
    };
  },
};
</script> -->

<!-- <script>
// Composition API - VUE 3
export default {
  setup: function () {
    const nomeProduto = "Caderno";
    const codigoProduto = "#321";
    return {
      nomeProduto,
      codigoProduto,
    };
  },
};
</script> -->

<script setup>
const nomeProduto = "Caderno";
const codigoProduto = "#321";
</script>
