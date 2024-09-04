<script setup>
import PrimeiroComponente from "./components/PrimeiroComponente.vue"
import ComDadosReativosPrimitivos from "./components/ComDadosReativosPrimitivos.vue"
import ComDadosReativosNaoPrimitivos from "./components/ComDadosReativosNaoPrimitivos.vue"
import DataBinding from "./components/DataBinding.vue";
import ComProps from "./components/ComProps.vue";
import EscutaEvento from "./components/EscutaEvento.vue";
import PropriedadesComputada from "./components/PropriedadesComputadas.vue";
import PropriedadesAssistidas from "./components/PropriedadesAssistidas.vue";
</script>

<template>
  <header>Estudo dos conceitos basicos do Vue.js</header>
  <PropriedadesAssistidas/>
  <PropriedadesComputada/>
  <EscutaEvento/>
  <ComProps item="borracha" :value="2.1"/>
  <ComProps item="lapis" :value="2.5"/>
  <ComDadosReativosNaoPrimitivos/>
  <ComDadosReativosPrimitivos/>
  <DataBinding/>
  <PrimeiroComponente/>
</template>

