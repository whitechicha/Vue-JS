<template>
    <h1>Счетчик с использованием Composition API</h1>
    <p>Счет: {{ count }}</p>
    <button @click="increment">+++</button>
    <button @click="decrement">---</button>
</template>

<script setup>
import { ref } from 'vue';
const count = ref(2)

</script>