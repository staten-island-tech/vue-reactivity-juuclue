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
  <div class="bowl">
    <div v-if="bowl.length === 0">
      <p> no items in bowl</p>
    </div>
    <div v-else>
      <div v-for="(ingredient) in bowl" :key="ingredient.name" class="ingredient">
      <h3> {{  ingredient.name }}</h3>
      <img :src="ingredient.img" alt=""/>
      
    </div>
    </div>
  </div>
</template>
<script setup>
import { defineProps } from 'vue';

const props= defineProps({
  bowl: array
})
</script>

<style scoped>
.bowl{
  background-color:rgb(131, 107, 107);
  width:30%;
  position:absolute;
  top:0; right:0;
  height:889vh;
}
</style>