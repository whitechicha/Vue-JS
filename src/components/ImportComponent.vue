<template>
    <h2>Тест работы инпута в Vue</h2>

    <button @click="showText = !showText">Показать Текст</button>
    <p v-if="showText">kiouiyutdtcjhvbljp[uyt7ifcljhvjknhigtrtyrsfghcjhvkjgufir6tdkxghcjhvguotrp6tdugchjhvkjgu;frp6udtlcgjh]</p>
    <p v-else>Нажми на кнопку выше</p>

</template>

<script setup>
    import { ref } from 'vue';

    const showText = ref(false)
</script>