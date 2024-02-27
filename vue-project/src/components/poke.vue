<template>
    <div class="card2">
    <h2>{{ Supply.name }}</h2>
    <img :src="Supply.img" alt=""/>

    <button @click="addToBowl(Supply)" class="button">Add to Bowl</button>

    </div>
    
</template>

<script setup>
import { data } from '@/stores/store.js'

 
const props = defineProps({
    Supply: Object,
});
const addToBowl = function (product){
    data.bowl.push(product)
}
/* const bowl=[];
function addToBowl(){
    bowl.push({
        name: props.Supply.name,
        img: props.Supply.img
    }       
    
    
    )
    console.log(bowl)

    
}  */




/* let clicked = ref(0);
function increment(){
    clicked.value++;
}
function decrement(){
    clicked.value--;
}
    <!-- <h3>{{ clicked }}</h3> --> */

/*  <button @click="decrement"> - </button>
    <button @click="increment"> + </button> */
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
.button{
    background-color:beige;
    border:3px solid rgb(102, 94, 86);
    border-radius:5px
}
</style >

