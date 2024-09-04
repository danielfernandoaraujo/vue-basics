<template>
    <div class="componente">
        <h1>Componente que emite evento</h1>
        <p>Nome: {{ item }} | Valor: R${{ value.toFixed(2) }}</p>
        <button @click="adicionar">Adicionar ao carrinho</button>
    </div>
</template>

<script setup>
import { defineProps, defineEmits } from 'vue';

const props = defineProps({
    item:String,
    value:Number
})

const emit = defineEmits(["foiAdicionado"])

function adicionar(){
    emit("foiAdicionado", props.value)
}

</script>

