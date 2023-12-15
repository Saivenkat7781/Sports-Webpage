<template>
  <div class="section" id="sectionOne">
    <h2>List of Players</h2>
    <div class="content">
      <ul>
        <li v-for="(item) in items" :key="item" @click="showDetails(item)">
           {{ item }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Section1',
  data() {
    return {
      items: [
        'Messi',
        'Ronaldo',
        'Lebron James',
        'Virat Kohli',
        'Roger Federer',
        'Rafael Nadal',
        'John Cena',
        'Tiger Woods',
        'Patrick Mahomes',
        'Usain Bolt',
      ],
      highlightedIndex: null,
    };
  },
  methods: {
    showDetails(item) {
      this.$emit('itemSelected', item);
    },
  },
};
</script>

<style scoped>
.section {
  flex: 1;
  overflow-y: auto;
  padding: 20px;
  border: 1px solid #ccc;
  margin: 10px;
  height: 300px; 
  font-family: sans-serif;
  font-weight: bold;
}

.content {
}

h2{
  background-color: #B2DFDB;
  font-size: 24px; 
  margin-bottom: 15px; 
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  margin-bottom: 8px;
  cursor: pointer;
  transition: background-color 0.4s ease;
}

li:hover {
  background-color: #e0e0e0; 
}
li.highlighted {
  background-color: #ffcc80; 
}
</style>
