<template>
    <div class="componente">
        <h1>Componente com propriedades Assistidas</h1>
        <p>Idade: {{ idade }}</p>
        <label>Ano de Nascimento:</label>
        <input type="number" v-model="anoNascimento" min="2000">
        <label>Ano Atual:</label>
        <input type="number" v-model="anoAtual" min="2000">
    </div>
</template>

<script setup>
import { ref, watchEffect } from 'vue';
const today = new Date();
const year = today.getFullYear()

const anoNascimento = ref(0)
const anoAtual = ref(year)
const idade = ref(0)

// Forma de usar o watch

// watch(anoAtual, (ano)=>{
//     idade.value = ano - anoNascimento.value
// })
// watch(anoNascimento, (ano)=>{
//     idade.value = anoAtual.value - ano 
// })

// Forma de usar o watch effect.

watchEffect(()=>{
    idade.value = anoAtual.value - anoNascimento.value
})

</script>

<style>
label{
    margin: 10px;
}
</style>