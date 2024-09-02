<template>
    <div class="componente">
        <h1>Componente com dados reativos primitivos</h1>
        <p>Nome: {{ productName }} | Value: {{ productValue }}</p>
        <button @click ="changeValue()">+</button>
    </div>
</template>

<script setup>
import {ref} from "vue"
// Ref avisa para o vue que pode mudar de valor

    const productName = "Laranja"
    const productValue = ref(1)

    function changeValue() {
        productValue.value += 2
    }
</script>
