<!-- <template>
  <div class="cards">
    <card2
      v-for="supply in bowl"
      :key="supply.name"
      :Supply="supply"
    />
  </div>

</template>

<script setup>
       

import card2 from "@/components/poke.vue";

import supply from "@/components/poke.vue";
console.log(bowl);
</script>
<style>
@media (min-width: 1024px) {
  .bowl {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style> -->
<template>
  <div class="body2">
  <h1> Your Bowl </h1>
  <div class="shopping">
    <div v-if="data.bowl.length === 0">
      <p>Make your Bowl!</p>
    </div>
    <div v-else>
      <div v-for="(Supply) in data.bowl" :key="Supply.name" class="stuff">
        <h2>{{ Supply.name }}</h2>
        <img :src="Supply.img" alt="" class="img"/>
        <button class="remove" @click="remove(Supply)">remove</button>
      </div>
    </div>
  </div>
</div>
</template>
<script setup>
  
  import { data } from '@/stores/store.js';

  const props = defineProps({
    bowl: Array
  
  })
 function remove(supply){
   const bowlIndex = data.bowl.indexOf(supply);
   data.bowl.splice(bowlIndex, 1);
   console.log(data.bowl); 
 }
</script>
<style scoped>
.body2{
  background-color:beige;
  width:35%;
  position:absolute;
  top:0; right:0;
  height: 889vh;
  text-align:center;
  align-items: center;
  justify-content: space-around;
  border:3px solid black;

}
.img{
    width: 150px;
    height: 100px;
    object-fit: cover;
    border:5px solid rgb(103, 86, 86);
    border-radius:5px;

}
.remove{
  background-color:rgb(159, 140, 140);
  border:5px solid rgb(230, 213, 191);
  border-radius:5px;
}
</style>
