<script setup>
/*import HelloWorld from './components/HelloWorld.vue'*/
/*import TheWelcome from './components/TheWelcome.vue'*/
import CustomComponent from './components/CustomComponent.vue'
</script>

<template>
  <CustomComponent />
<header>   
  </header>

<main>
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

}
</style>
