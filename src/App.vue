<script>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import CustomComponent from './components/CustomComponent.vue'

import worksData from './assets/works.json'

export default {
  data() {
    return {
      works: worksData,
    };
  },
  components: {
   CustomComponent,
  },
};

</script>

<template>
<header>   
  </header>

<main>
      <div class="row">
        <div class="col" v-for="work in works" :key="work.id">
           <CustomComponent 
            :title="work.title"
            :abstract="work.description"
            :imageUrl="work.image_thumbnail"
          />
        </div>
      </div> 
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
