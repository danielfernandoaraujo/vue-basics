<script setup>
import PrimeiroComponente from "./components/PrimeiroComponente.vue"
import ComDadosReativosPrimitivos from "./components/ComDadosReativosPrimitivos.vue"
import ComDadosReativosNaoPrimitivos from "./components/ComDadosReativosNaoPrimitivos.vue"
import DataBinding from "./components/DataBinding.vue";
</script>

<template>
  <ComDadosReativosNaoPrimitivos/>
  <ComDadosReativosPrimitivos/>
  <PrimeiroComponente/>
  <DataBinding/>
</template>

<style scoped>

</style>
