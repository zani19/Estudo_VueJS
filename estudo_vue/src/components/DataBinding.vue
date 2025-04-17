<template>
    <div class="componente">
        <h1>Componente de Data Binding</h1>
        <p>{{ valor }}</p>
        <!-- <input type="text" v-bind:value="valor"></input> -->

        <!-- <input type="text" v-bind:value="valor" v-on:input="(e)=>valor = e.target.value"></input> -->

        <!-- com atalhos v-bind e v-on -->
        <input type="text" :value="valor" @:input="(e)=>valor = e.target.value"></input>
    </div>
</template>

<script setup>
import { ref } from "vue";
const valor = ref("Vue 3.0.0");
</script>