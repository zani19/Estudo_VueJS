<script setup>
import ComDados from "./components/ComDados.vue";
import ComDadosReativosNaoPrimitivos from "./components/ComDadosReativosNaoPrimitivos.vue";
import ComDadosReativosPrimitivos from "./components/ComDadosReativosPrimitivos.vue";
import ComProps from "./components/ComProps.vue";
import DataBinding from "./components/DataBinding.vue";
import EscutaEvento from "./components/EscutaEvento.vue";
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import PropriedadesAssistidas from "./components/PropriedadesAssistidas.vue";
import PropriedadesComputadas from "./components/PropriedadesComputadas.vue";
import RenderizacaoCondicional from "./components/RenderizacaoCondicional.vue";
</script>

<template>
  <header>Vue</header>
  <RenderizacaoCondicional nome="Thiago" :qtdeCachorros="2"/>
  <PropriedadesAssistidas />
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
