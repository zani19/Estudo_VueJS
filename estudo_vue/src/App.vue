<script setup>
import ComDados from "./components/ComDados.vue";
import ComDadosReativosNaoPrimitivos from "./components/ComDadosReativosNaoPrimitivos.vue";
import ComDadosReativosPrimitivos from "./components/ComDadosReativosPrimitivos.vue";
import ComProps from "./components/ComProps.vue";
import DataBinding from "./components/DataBinding.vue";
import EscutaEvento from "./components/EscutaEvento.vue";
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import PropriedadesComputadas from "./components/PropriedadesComputadas.vue";
</script>

<template>
  <header>Vue</header>
  <PropriedadesComputadas />
  <EscutaEvento />
  <ComProps item="Borracha" :preco="2.50"/>
  <DataBinding/>
  <ComDadosReativosNaoPrimitivos />
  <ComDadosReativosPrimitivos />
  <ComDados />
  <PrimeiroComponente />
</template>

<style scoped></style>
