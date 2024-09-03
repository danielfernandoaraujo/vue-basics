<template>
    <div class="componente">
        <h1>Componente com dados reativos não primitivos</h1>
        <p>Nome: {{ person.name }} | Idade: {{ person.age }}</p>
        <button @click ="changeValue()">+</button>
    </div>
</template>

<script setup>
import {reactive} from "vue"
// Ref avisa para o vue que pode mudar de valor

const person = reactive({name: "Daniel", age:5})

function changeValue() {
    person.age += 1
}

</script>
