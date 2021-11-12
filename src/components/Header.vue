<template>
  <header class="container">
      <nav>
          <img src="../assets/img/dc-logo.png" alt="dc-logo">
          <ul>
             <li v-for="(element, i) in navLinks" :key="i" ><a :href="element.src" @click.prevent="currentTab = i">{{element.txt}}</a>
             <div :class="i === currentTab ? 'active' : ''"></div></li> 
          </ul>
      </nav>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data(){
        return {
            currentTab: 0,
            navLinks: [
            {
                txt: "CHARACTERS",
                src: "#"
            },
            {
                txt: "COMICS",
                src: "#"
            },
            {
                txt: "MOVIES",
                src: "#"
            },
            {
                txt: "TV",
                src: "#"
            },
            {
                txt: "GAMES",
                src: "#"
            },
            {
                txt: "COLLECTIBLES",
                src: "#"
            },
            {
                txt: "VIDEOS",
                src: "#"
            },
            {
                txt: "FANS",
                src: "#"
            },
            {
                txt: "NEWS",
                src: "#"
            },
            {
                txt: "SHOP",
                src: "#"
            },
        ]
        }
    }
    }
</script>

<style>

</style>