<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="title">
    <h1>Smile more</h1>
    <link rel="stylesheet" href="https://use.typekit.net/ifs2uyi.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
     <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
      <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@100&display=swap" rel="stylesheet">
     </div>
    <div>
    <img class="img-smile" src="smile.png" alt="">
    </div>
    <div>
      <p>Il sorriso è molto importante perché rafforza i legami sociali,</p>
        <p>dona una sensazione di benessere a noi e agli altri.</p>
        <p>Le endorfine sono le sostanze che ci fanno sentire felici</p>
        <p>e meno stressati, inducendo una sensazione di calma e tranquillità.</p>
    </div>
    
</template>

<style scoped>
.title {
  display: flex;
  align-items: center;
}
h1 {
  color: rgb(255, 255, 255);
  font-family: fino-sans, sans-serif;
  font-style: normal;
  font-size: 100px;
}
.img-smile {
width: 100px;
margin-top: 1.5rem;
}
p {
  font-family:'Poppins', sans-serif;
  color: white;
  font-size: medium;
}
</style>
