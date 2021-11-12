<template>
  <main>
    <div class="container">
      <p>--> Content goes here &#60;--</p>
    </div>
  </main>
</template>

<script>
import jsonData from '@/assets/dc-comics.json'

export default {
  name: "Main",
  data(){
    return {
      dcList: jsonData,
    }
  }
};
</script>

<style>
</style>