<template>
    <header>
        <div class="headerline">
            <div class="block-header-one">
                <p>Summer Sale For All Swim Suits And Free Express Delivery - OFF 50%!</p>
                <a href="#" class="Show_text">ShopNow</a>
            </div>

            <div class="block-header-one dropdown">

                <button class="button_language" @click="show_language = !show_language">{{ langLabel }} ↓</button>
                <ul class="" v-show="show_language">
                    <li><button class="button_language" @click="changeLangLabel">Russain</button></li>
                    <li><button class="button_language" @click="changeLangLabel">Армянский</button></li>
                    <li><button class="button_language" @click="changeLangLabel">Грузинский</button></li>
                    <li><button class="button_language" @click="changeLangLabel">Russain</button></li>
                </ul>
            </div>
        </div>
        <div class="block-header-two ">
            <h1>Exclusive </h1>
            <div class="button-header">
                <a class="link_words" href="#">Home</a>
                <a class="link_words" href="#">Contact</a>
                <a class="link_words" href="#">About</a>
                <a class="link_words" href="#">Sing up</a>
            </div>


            <div class="input_img">
                <div class="input_header">
                    <input class="input-one" type="text" placeholder="What are you looking for?">
                    <img class="img_one" src="../assets/img/pngwing.com.png" alt="">
                </div>
                <div class="img_first">
                    <a href=""><img src="../assets/img/pngwing.com (1).png" alt=""></a>
                    <a href=""><img src="../assets/img/pngwing.com (2).png" alt=""></a>
                </div>
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
    margin: -10px;

}

.input_img {
    display: flex;
    column-gap: 20px;
}

.block-header-one {
    display: flex;
    padding: auto;
    color: white;
    margin: 10px;
    position: relative;
    align-items: center;
}




.img_first {
    display: flex;
    align-items: center;
    column-gap: 20px;
}

.img_first img {
    width: 25px;
    height: 25px;
}

.button_language {
    background-color: #ffffff00;
    color: white;

}

.dropdown ul {
    position: absolute;
    top: 100%;

    color: #000;
    background-color: white;
    box-shadow: 2px 2px 10px #00000032;
    padding: 10px;
    list-style: none;

    display: flex;
    flex-direction: column;
    row-gap: 10px;
}

.dropdown ul .button_language {
    color: #000;
    cursor: pointer;
}



.Show_text {
    display: flex;
    padding-right: 50px;
    padding-left: 20px;
    color: white;
}

.img_two {
    width: 32px;
    height: 32px;
}

.block-header-two  {
    display: flex;
    align-items: center;
    justify-content: space-between;
    max-width: 1170px;
    margin: 0 auto;
    margin-top: 40px;
}

.input_header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: #F5F5F5;
    width: 243px;
    height: 38px;
    border-radius: 4px;
    border: solid rgb(235, 235, 235) 1px;
}

.img_one {
    width: 24px;
    height: 24px;
}

.input-one {
    background-color: #F5F5F5;
    color: rgb(0, 0, 0);
    border: none;
}

.link_words {
    display: flex;
    padding: 0 30px 0 30px;
    font-size: 20px;
    color: black;
    text-decoration: none;
}

.input-one {
    outline: none;
    width: 210px;
}

.button-header {
    display: flex;
    align-items: center;
}
</style>
