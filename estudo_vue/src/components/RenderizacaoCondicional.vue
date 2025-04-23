<template>
    <div class="componente">
        <h1>Renderização Condicional</h1>
        <p v-if="idade >= 18">Maior de Idade</p>
        <h1>Componente com Renderização Condicional</h1>
        <p>Nome: {{ nome }}</p>
        <p v-if="qtdeCachorros===0">Não tem cachorro</p>
        <p v-else-if="qtdeCachorros===1">Tem um cachorro</p>
        <p v-else>Tem muitos Cachorros</p>
    </div>
</template>

<script setup>
import { defineProps } from 'vue';

defineProps ({
    nome: String,
    qtdeCachorros: Number
})
</script>