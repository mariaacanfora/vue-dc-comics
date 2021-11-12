<template>
  <main>
    <div class="main-hero">

    </div>

    <div class="container">
      <div class="label-cs">
        CURRENT SERIES
      </div>

      <Card v-for="(card, i) in dcList" :key="i" :img="card.thumb" :title="card.series.toUpperCase()">
        
      </Card>
    </div>
  </main>
</template>

<script>
import jsonData from "@/assets/dc-comics.json";
import Card from "./Card.vue"

export default {
  name: "Main",
  components: {
    Card
  },
  data() {
    return {
      dcList: jsonData,
    };
  },
};
</script>

<style>
</style>