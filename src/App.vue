<script setup>
import PrimeiroComponente from "./components/PrimeiroComponente.vue"
import ComDadosReativosPrimitivos from "./components/ComDadosReativosPrimitivos.vue"
import ComDadosReativosNaoPrimitivos from "./components/ComDadosReativosNaoPrimitivos.vue"
import DataBinding from "./components/DataBinding.vue";
import ComProps from "./components/ComProps.vue";
import EscutaEvento from "./components/EscutaEvento.vue";
</script>

<template>
  <ComProps item="borracha" :value="2.1"/>
  <ComProps item="lapis" :value="2.5"/>
  <ComDadosReativosNaoPrimitivos/>
  <ComDadosReativosPrimitivos/>
  <PrimeiroComponente/>
  <DataBinding/>
</template>

<style scoped>

</style>
