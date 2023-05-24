<script>
import Header from './components/Header.vue'
import CustomComponent from './components/CustomComponent.vue'

import worksData from './assets/works.json'

export default {
  data() {
    return {
      works: worksData,
    };
  },
  components: {
    Header,
    CustomComponent,
  },
};

</script>

<template>
<main>
  <header>

  </header>
      <div class="row">
        <div class="col-12 col-md-6" v-for="work in works" :key="work.id">
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
