<script setup>
defineProps({
  title: String,
  abstract: String,
  imageUrl: String,
})
</script>

<template>
   <div class="section" >
    <div class="image">
      <img :src="imageUrl" width="200" height="250">
      <h2 class="title" >{{ title }}</h2> 
      <p class="description">
        {{ abstract }}
      </p>
    </div>
   </div>    
</template>

<style scoped>
  .title {
    font-size: 2em;
  }
  .custom-component {
    background-color: v-bind(color);
  }
  .image {
    margin-top: 40px;
  }
</style>
