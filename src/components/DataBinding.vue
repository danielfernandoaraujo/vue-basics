<template>
    <div class="componente">
        <h1>Data Biding</h1>
        <p>{{ valor }}</p>
        <!-- Essa é a forma mais verbosa -->

        <!-- <input type="text" v-bind:value="valor"
        v-on:input="(e)=>valor = e.target.value"
        ></input> -->

        <!-- Essa é a forma mais limpa -->
         
        <input type="text" v-model="valor"
        ></input>
    </div>
</template>

<script setup>
import {ref} from "vue"
const valor = ref("Digite seu nome aqui")
</script>
