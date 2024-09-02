<template>
    <div class="componente">
        <h1>Componente com dados reativos não primitivos</h1>
        <p>Nome: {{ pessoa.nome }} | Valor: {{ pessoa.idade }}</p>
        <button @click ="changeValue()">+</button>
    </div>
</template>

<script setup>
import {reactive} from "vue"
// Ref avisa para o vue que pode mudar de valor

const pessoa = reactive({nome: "Daniel", idade:5})

function changeValue() {
    pessoa.idade += 1
}

</script>
