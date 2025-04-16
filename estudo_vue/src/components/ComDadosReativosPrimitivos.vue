<template>
  <div class="componente">
    <h1>Componente com Dados Reativos Primitivos<br /></h1>
    <p>Nome: {{ nome }} | Idade: {{ idade }}</p>
    <button v-on:click="fazerAniversario()">Fazer Aniverário</button>
    <button @click="mudarNome()">Alterar Nome</button>    
</div>
</template>

<script setup>
import { ref } from "vue";
const nome = ref ("Thiago");
const idade = ref (41);

function fazerAniversario (){
    idade.value ++;
}

function mudarNome (){
    nome.value = "Thiago Silva";
}

</script>
