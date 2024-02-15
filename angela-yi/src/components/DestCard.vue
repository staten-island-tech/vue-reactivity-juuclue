<template>
    <div class ="card2">
    <h2>{{ Supply.name }}</h2>
    <img :src="Supply.img" alt=""/>
    <h3>{{ clicked }}</h3>
    <button @click="decrement"> - </button>
    <button @click="increment"> + </button>
    </div>
</template>
<script setup>
import { ref } from "vue";
const props = defineProps({
    Supply: Object,
});

let clicked = ref(0);
function increment(){
    clicked.value++;
}
function decrement(){
    clicked.value--;
}

</script>

<style scoped>
img {
    width:  310px;
    height: 260px;
    object-fit: cover;
}
.card2 {
    background-color: antiquewhite;
    margin-top:5vh;
    margin-bottom:5vh;
    margin-left:0vs;
    width:70%;
    padding-top:2vh;
    padding-bottom: 2vh;
    border-radius:5vh;
    display:flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: space-around;
    align-content:center;

}
.cards{
    display:flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: space-around;
    align-content:center;
}
</style>