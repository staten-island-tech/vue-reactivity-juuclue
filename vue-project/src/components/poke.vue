<template>
    <div class="card2">
    <h2>{{ Supply.name }}</h2>
    <img :src="Supply.img" alt=""/>
    <!-- <h3>{{ clicked }}</h3> -->
    <button>Add to Bowl</button>
<!--     <button @click="decrement"> - </button>
    <button @click="increment"> + </button> -->
    </div>
</template>

<script setup>
import { ref } from "vue";
const props = defineProps({
    Supply: Object,
});

/* const bowl=[]
addtoBowl(Supply);
bowl.push(Supply) */
/* let clicked = ref(0);
function increment(){
    clicked.value++;
}
function decrement(){
    clicked.value--;
} */


</script>


<style scoped>

img {
    width:  150px;
    height: 100px;
    object-fit: cover;
}
.card2 {
    background-color: rgb(204, 191, 174);
    margin-top:5vh;
    margin-bottom: 2vh;
    margin-left:0vs;
    width:70%;
    padding-top:2vh;
    padding-bottom: 2vh;
    border-radius:5vh;
    text-align: center;
}
</style >

