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
  <div class="shopping">
    <div v-if="data.bowl.length === 0">
      <p>Make your Bowl!</p>
    </div>
    <div v-else>
      <div v-for="(stuff) in data.bowl" :key="stuff.name" class="stuff">
        <h2>{{ stuff.name }}</h2>
        <img :src="stuff.img" alt=""/>
      </div>
    </div>
  </div>
</template>
<script setup>
  import {defineProps} from 'vue';
  import { data } from 'vue';
  import {ref} from 'vue';
  const props = defineProps({
    bowl: Array
  })
</script>
