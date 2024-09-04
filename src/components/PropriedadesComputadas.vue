<template>
    <div class="componente">
        <h1>Componente com propriedades computadas</h1>
        <p>Idade: {{ idade }}</p>
        <label>Ano de Nascimento:</label>
        <input type="number" v-model="anoNascimento" min="2000">
        <label>Ano Atual:</label>
        <input type="number" v-model="anoAtual" min="2000">
    </div>
</template>

<script setup>
import { ref, computed } from 'vue';
const today = new Date();
const year = today.getFullYear()

const anoNascimento = ref(2004)
const anoAtual = ref(year)
const idade = computed(()=>{
    return anoAtual.value - anoNascimento.value
})

</script>

<style>
label{
    margin: 10px;
}
</style>