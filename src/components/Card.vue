<template>
  <div class="card-col">
    <div class="img-container">
      <img
        :src="img"
        :alt="title"
      />
    </div>
    <p class="card-title"> {{title}} </p>
  </div>
</template>

<script>
export default {
  name: "Card",
  props:  ["img", "title"]
};
</script>

<style lang="scss">
@import "@/styles/variables.scss";
.card-col {
  width: calc(100% / 6 - $padding-x * 2.05);

  .img-container {
    height: $max-width-container / 6;
    overflow: hidden;
  }

  img {
    width: 100%;
  }

  .card-title{
      padding: $padding-y 0;
  }
}
</style>