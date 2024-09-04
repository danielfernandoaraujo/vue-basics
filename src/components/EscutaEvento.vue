<template>
    <div class="componente">
        <h1>Componente que escuta evento</h1>
        <p>Total: R${{ total }}</p>
        <div class="lista">
            <EmiteEvento item="batata" :value="1.99" @foiAdicionado="atualizarTotal"/>
            <EmiteEvento item="feijão" :value="2.99" @foiAdicionado="atualizarTotal"/>
            <EmiteEvento item="água" :value="4.99" @foiAdicionado="atualizarTotal"/>
        </div>
            <button @click="limparCarrinho">Limpar carrinho</button>
    </div>
</template>

<script setup>
import EmiteEvento from './EmiteEvento.vue';
import { ref } from 'vue';
const total = ref(0)

function atualizarTotal(p){
    const valor = total.value + p
    total.value = +valor.toFixed(2)

}

function limparCarrinho(p){
    total.value = 0

}

</script>
