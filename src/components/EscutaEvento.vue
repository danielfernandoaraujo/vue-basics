<template>
    <div class="componente">
        <h1>Componente que escuta evento</h1>
        <p>Total: R$ {{ total }}</p>
        <div>
            <EmiteEvento item="Item1" :preco="1.99"></EmiteEvento>
            <EmiteEvento item="Item2" :preco="2.99"></EmiteEvento>
            <EmiteEvento item="Item1" :preco="4.99"></EmiteEvento>
        </div>
    </div>
</template>

<script setup>
import EmiteEvento from './EmiteEvento.vue';

</script>
