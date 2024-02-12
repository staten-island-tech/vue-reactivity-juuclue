
<template>
  <div class ="cards">
        <DestCard
      v-for="supply in supplys"
      :key="supply.name"
      :Supply="supplys"
    />
  </div>
</template>

<script setup>
import DestCard from "@/components/DestCard.vue";
const supplys = [
 {
  name: "Nori(shredded)",
  img: "https://gimlifish.com/cdn/shop/products/noriseaweedwraps_530x@2x.jpg?v=1592063167",
 },
 {
  name: "sushi rice",
  img: "https://simplyhomecooked.com/wp-content/uploads/2022/06/sushi-rice-recipe-2.jpg",
 },
 {
  name: "avocado",
  img: "https://media.istockphoto.com/id/179301015/photo/close-up-of-fresh-ripe-avocado-slices-on-white-background.jpg?s=612x612&w=0&k=20&c=LSGBs32WzLdfwZ-zDyZ5ocU3GiwZxrMbk96thjm3Ykk=",
 },
 {
  name: "Salmon",
  img: "https://umamicart.com/cdn/shop/products/salmon-sashimi_grande.png?v=1692355095",
 },
 {
  name: "Tuna",
  img: "https://wagyuman.com/cdn/shop/products/wagyuman-seafood-1-5-lbs-24-0-oz-chutoro-blue-fin-tuna-16487795294305_1200x1200.jpg?v=1627998293",
 },
 {
  name: "Cucumber",
  img: "https://www.wikihow.com/images/thumb/2/2a/Make-Sushi-Step-13.jpg/550px-nowatermark-Make-Sushi-Step-13.jpg",
 },
 {
  name: "Roe",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Soba noodles",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Zucchini noodles",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "brown rice",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "negitoro",
  img: "https://storage.googleapis.com/duckr-b8e76.appspot.com/resized/FgbFY0Csq-f8c277eadfcd2d954c3f9908e498d7fa262b1dc4bb49a07d25d8aa10af00eeee_896x504.jpg",
 },
 {
  name: "Spring mix",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "spicy tuna",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Spicy salmon",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Shrimp",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "chicken",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "organic tofu",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "yellowtail",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Unagi(EEL)",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "grilled salmon",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "teriyaki beef",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Cilantro",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "hijiki seaweed",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Jalapeno",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "sweet corn",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Sweet onion",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "carrot",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Cilantro Ranch",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "House Poke sauce",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "lemon ponzu",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "spicy poke sauce",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "sesame shoyu",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Spicy mayo",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Sweet unagi sauce",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "honey dijon sauce",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Teriyaki sauce",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "cucumber",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Edamame",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "seaweed salad",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Cherry tomatoes",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Chopped Mango",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Sweet Ginger",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Masago",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Spicy Crab Salad",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Radish",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Pineapple",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Wasabi",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "garlic crisps",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "double avocado",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "sesame mix",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "onion crisps",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Wonton crisps",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Purple cabbage",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "Wasabi Aiolio",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },
 {
  name: "crab salad",
  img: "https://www.markys.com/media/catalog/product/cache/b0d56cdde5a8ef6c30b52cc73236630f/0/1/014202-01_v0ec04odvsbf18ed.jpg",
 },

 


]
</script>
