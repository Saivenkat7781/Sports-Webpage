<template>
  <div id="app">
    <Header />
    <div class="sections-container">
    <Section1 @itemSelected="updateSelectedItem" />
    <Section2 :selectedItem="selectedItem" />
    <Section3 :selectedItem="selectedItem" />
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Section1 from './components/SectionOne.vue';
import Section2 from './components/SectionTwo.vue';
import Section3 from './components/SectionThree.vue';

export default {
  name: 'App',
  components: {
    Header,
    Section1,
    Section2,
    Section3,
  },
  data() {
    return {
      selectedItem: '',
    };
  },
  methods: {
    updateSelectedItem(item) {
      
      this.selectedItem = item;
    },
  },
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  
  color: black;
  display: flex;
  flex-direction: column;
  background-image: url('D:\Photos\Add.jpg'); 
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  display: flex;
  height: 100vh;
}

@media screen and (max-width: 768px) {
  .background-image {
    opacity: 0.4;
  }
}

.sections-container {
  display: flex;
  justify-content: center; 
  margin: 20px;
}

.sections {
    flex-direction: column; 
  }
</style>
