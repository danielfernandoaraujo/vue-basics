<template>
    <div class="componente">
        <h1>Componente com Props</h1>
        <p>Nome: {{ item }} | Valor: {{ value.toFixed(2) }}</p>
    </div>
</template>

<script setup>
// Passar informações do componente pai para o filho

import { defineProps } from 'vue';

defineProps({
    item:String,
    value:Number
})
</script>
