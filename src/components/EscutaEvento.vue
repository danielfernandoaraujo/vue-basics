<template>
    <div class="componente">
        <h1>Componente que escuta evento</h1>
        <p>Total: R${{ total }}</p>
        <div class="lista">
            <EmiteEvento item="batata" :value="1.99"/>
            <EmiteEvento item="feijão" :value="2.99"/>
            <EmiteEvento item="água" :value="4.99"/>
        </div>
    </div>
</template>

<script setup>
import EmiteEvento from './EmiteEvento.vue';

</script>
