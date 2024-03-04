<template>
<header>
    <div class="headerline">
        <p>Summer Sale For All Swim Suits And Free Express Delivery - OFF 50%! <a href="#">ShopNow</a> </p>

        <div class="button">
            <button class="button_language" @click="show_language = !show_language">{{ langLabel }} -></button>
                <ul v-show="show_language">
                    <li><button class="button_language" @click="changeLangLabel">Russain</button></li>
                    <li><button class="button_language" @click="changeLangLabel">French</button></li>
                    <li><button class="button_language" @click="changeLangLabel">Germany</button></li>
                    <li><button class="button_language" @click="changeLangLabel">Japanese</button></li>
            </ul>
        </div>
    </div>

    <div class="header-main">
        <div class="Sell">
            <h1>Exclusive</h1>
        </div>

        <div class="button-header">
            <a href="#">Home</a>
            <a href="#">Contact</a>
            <a href="#">About</a>
            <a href="#">Sing up</a>
        </div>

        <div class="button-icon">
            
        </div>
    </div>
</header>
</template>

<script setup>
import { ref } from 'vue';

function changeLangLabel(e) {   
    langLabel.value = e.target.textContent
}

const show_language = ref(true)
const langLabel = ref('English')
</script>

<style scoped>
    .headerline {
        display: flex;
        justify-content: space-around;
        background-color: black;
        color: white;
        margin: -10px;
    }

    .headerline a {
        color: white;
    }

    .button {

    }
</style>