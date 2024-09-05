<template>
    <div class="componente">
        <h1>Componente com renderização condicional</h1>
        <p>Nome: {{ nome }}</p>
        <p v-if="qntdeCachorros === 0">Não tem cachorros</p>
        <p v-else-if="qntdeCachorros === 1">Tem um cachorro</p>
        <p v-else>Tem muitos cachorros</p>
    </div>
</template>

<script setup>
import { defineProps } from 'vue';

defineProps({
    nome: String,
    qntdeCachorros: Number
})
</script>