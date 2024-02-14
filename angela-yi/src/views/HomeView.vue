
<template>
  <div class ="cards">
        <card2
      v-for="supply in supplys"
      :key="supply.name"
      :Supply="supply"
    />
  </div>
</template>

<script setup>
import card2 from "@/components/DestCard.vue";
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
  img: "https://www.chopstickchronicles.com/wp-content/uploads/2021/03/Soba-Noodle-10.webp",
 },
 {
  name: "Zucchini noodles",
  img: "https://www.wholesomeyum.com/wp-content/uploads/2021/06/wholesomeyum-Zucchini-Noodles-Recipe-Zoodles-15.jpg",
 },
 {
  name: "brown rice",
  img: "https://media.post.rvohealth.io/wp-content/uploads/2023/09/brown-rice-header.jpg",
 },
 {
  name: "negitoro",
  img: "https://storage.googleapis.com/duckr-b8e76.appspot.com/resized/FgbFY0Csq-f8c277eadfcd2d954c3f9908e498d7fa262b1dc4bb49a07d25d8aa10af00eeee_896x504.jpg",
 },
 {
  name: "Spring mix",
  img: "https://foolproofliving.com/wp-content/uploads/2022/03/Spring-Mix-Salad-Recipe.jpg",
 },
 {
  name: "spicy tuna",
  img: "https://www.savorysweetspoon.com/wp-content/uploads/2023/07/Spicy-Tuna-3-960x1200.jpg",
 },
 {
  name: "Spicy salmon",
  img: "https://www.tastingtable.com/img/gallery/spicy-honey-glazed-salmon-recipe/l-intro-1644519469.jpg",
 },
 {
  name: "Shrimp",
  img: "https://www.cookingforkeeps.com/wp-content/uploads/2023/03/Shrimp-Poke-Bowls-Web-3-1024x683.jpg.webp",
 },
 {
  name: "chicken",
  img: "https://www.foodservicedirect.com/media/catalog/product/1/0/10038034052495_2.jpg?width=1200&height=1200&quality=85&fit=bounds",
 },
 {
  name: "organic tofu",
  img: "https://hurrythefoodup.com/wp-content/uploads/2021/12/sesame-tofu-vegan-poke-bowl-in-progress.jpg",
 },
 {
  name: "yellowtail",
  img: "https://thetopmeal.com/wp-content/uploads/2022/11/hamachi-poke-3.jpg",
 },
 {
  name: "Unagi(EEL)",
  img: "https://cdn.media.amplience.net/i/japancentre/recipe-1434-unagi-don-grilled-eel-rice-bowl/recipe-1434-unagi-don-grilled-eel-rice-bowl?$poi$&w=700&h=410&sm=c&fmt=auto",
 },
 {
  name: "grilled salmon",
  img: "https://feelgoodfoodie.net/wp-content/uploads/2021/06/how-to-grill-salmon-8.jpg",
 },
 {
  name: "teriyaki beef",
  img: "https://www.slimmingeats.com/blog/wp-content/uploads/2016/06/beef-teriyaki-4-1.jpg",
 },
 {
  name: "Cilantro",
  img: "https://healthiersteps.com/wp-content/uploads/2021/11/cilantro-bunch.jpg",
 },
 {
  name: "hijiki seaweed",
  img: "https://www.maindish.in/wp-content/uploads/2020/09/hijiki_main2.jpg",
 },
 {
  name: "Jalapeno",
  img: "https://measianfoods.com/cdn/shop/products/jalapeno.png?v=1646605821",
 },
 {
  name: "sweet corn",
  img: "https://www.jiomart.com/images/product/original/590001511/sweet-corn-shelled-200-g-pack-product-images-o590001511-p590335340-0-202203171044.jpg?im=Resize=(1000,1000)",
 },
 {
  name: "Sweet onion",
  img: "https://www.seriouseats.com/thmb/6lQgiWc9s0tLibRrf_85CJY9mco=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/__opt__aboutcom__coeus__resources__content_migration__serious_eats__seriouseats.com__images__2016__06__20160608-poke-tuna-hamachi-octopus-salmon-hawaii-recipe-02-fe42fe8c18e64a72b85c4cb2f11b84cc.jpg",
 },
 {
  name: "carrot",
  img: "https://hentick.com/cdn/shop/files/carrots_600x.jpg?v=1686035952",
 },
 {
  name: "Cilantro Ranch",
  img: "https://www.chelseasmessyapron.com/wp-content/uploads/2022/08/Healthy-Cilantro-Lime-Dressing-1.jpeg",
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
