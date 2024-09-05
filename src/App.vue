<script setup>
import PrimeiroComponente from "./components/PrimeiroComponente.vue"
import ComDadosReativosPrimitivos from "./components/ComDadosReativosPrimitivos.vue"
import ComDadosReativosNaoPrimitivos from "./components/ComDadosReativosNaoPrimitivos.vue"
import DataBinding from "./components/DataBinding.vue";
import ComProps from "./components/ComProps.vue";
import EscutaEvento from "./components/EscutaEvento.vue";
import PropriedadesComputada from "./components/PropriedadesComputadas.vue";
import PropriedadesAssistidas from "./components/PropriedadesAssistidas.vue";
import RenderizacaoCondicional from "./components/RenderizacaoCondicional.vue";
import RenderizacaodeListas from "./components/RenderizacaodeListas.vue";
import Slots from "./components/Slots.vue";

const cachorrosDoDaniel = [
  {nome: "Totó", idade:2},
  {nome: "Laika", idade:4},
  {nome: "Lupita", idade:5}
]
</script>

<template>
  <header>Estudo dos conceitos basicos do Vue.js</header>
  <Slots>
    <template v-slot:icone>
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="currentColor"
      class="icon icon-tabler icons-tabler-filled icon-tabler-alert-octagon">
      <path stroke="none" d="M0 0h24v24H0z" fill="none" />
      <path
        d="M14.897 1a4 4 0 0 1 2.664 1.016l.165 .156l4.1 4.1a4 4 0 0 1 1.168 
        2.605l.006 .227v5.794a4 4 0 0 1 -1.016 2.664l-.156 .165l-4.1 4.1a4 4 0 0 1 -2.603 1.168l-.227 .006h-5.795a3.999 3.999 
        0 0 1 -2.664 -1.017l-.165 -.156l-4.1 -4.1a4 4 0 0 1 -1.168 -2.604l-.006 -.227v-5.794a4 4 0 0 1 1.016 -2.664l.156 -.165l4.1 
        -4.1a4 4 0 0 1 2.605 -1.168l.227 -.006h5.793zm-2.887 14l-.127 .007a1 1 0 0 0 0 1.986l.117 .007l.127 -.007a1 1 0 0 0 0 -1.986l-.117 -.007zm-.01 -8a1 1 0 0 0 -.993 .883l-.007 
        .117v4l.007 .117a1 1 0 0 0 1.986 0l.007 -.117v-4l-.007 -.117a1 1 0 0 0 -.993 -.883z" />
    </svg>
    </template>

  </Slots>
  <RenderizacaodeListas nome="Daniel" :cachorros="cachorrosDoDaniel" />
  <RenderizacaoCondicional nome="Daniel" :qntdeCachorros="1" />
  <PropriedadesAssistidas />
  <PropriedadesComputada />
  <EscutaEvento />
  <ComProps item="borracha" :value="2.1" />
  <ComProps item="lapis" :value="2.5" />
  <ComDadosReativosNaoPrimitivos />
  <ComDadosReativosPrimitivos />
  <DataBinding />
  <PrimeiroComponente />
</template>

