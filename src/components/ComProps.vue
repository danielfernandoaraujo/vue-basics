<template>
    <div class="componente">
        <h1>Componente com Props</h1>
        <p>Nome: {{ productName }} | Value: {{ productValue }}</p>
        <button @click ="changeValue()">+</button>
    </div>
</template>

<script setup>
import {ref} from "vue"

</script>
