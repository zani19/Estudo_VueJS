<template>
  <div class="componente">
    <h1>Componente com Dados Reativos Não Primitivos<br /></h1>
    <p>Nome: {{ pessoa.nome }} | Idade: {{ pessoa.idade }}</p>
    <button @click="fazerAniversario()">Fazer Aniverário</button>
    <button @click="mudarNome()">Alterar Nome</button>    
</div>
</template>

<!-- <script setup>
import { reactive } from "vue";

const pessoa = reactive({
    nome: "Thiago Zani",
    idade: 41
});

function fazerAniversario (){
    pessoa.idade ++;
}

function mudarNome (){
    pessoa.nome = "Thiago Silva";
}

</script> -->

<script>
export default {
    data: function (){
        return {
            pessoa: {
                nome: "Thiago Zani",
                idade: 41
            }
        };
    },
    methods: {
        fazerAniversario: function() {
            this.pessoa.idade++;
        },
        mudarNome: function() {
            this.pessoa.nome = "Thiago Silva";
        }
    }
};
</script>
