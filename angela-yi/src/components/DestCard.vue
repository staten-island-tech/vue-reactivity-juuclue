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
    height:40%;
    width: 50%;
    flex-direction: wrap;
}</style>