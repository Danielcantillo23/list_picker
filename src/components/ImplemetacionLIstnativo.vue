<template>
    <div>
      <VueListPickerNativa 
        :left-items="leftItems"
        :right-items="rightItems"
        titleLeft="items 1"
        v-model="selectedItems"
        titleRight="items 2"
      />
    </div>
  </template>
  
  <script>
  import VueListPickerNativa from './VueListPickerNativa.vue'
  export default {
    components: {
      VueListPickerNativa,
    },
    data() {
      const example1 = {
        key: 1,
        content: 'Item 1'
      }
      const example2 = {
        key: 2,
        content: 'Item 2'
      }
      const example3 = {
        key: 3,
        content: 'Item 3'
      }
      const example4 = {
        key: 4,
        content: 'Item 4'
      }
      
      const leftItems = [example1, example2]
      const rightItems = [example3, example4]
  
      return {
        leftItems,
        rightItems,
        selectedItems: [] 
      }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  h3 {
    margin: 40px 0 0;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  }
  </style>
  