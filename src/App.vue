<template>
  <div id="app">
    <Home v-bind:todos="todos"/>
  </div>
</template>

<script>

import Home  from "./components/Home";
export default {
  name: 'App',
  components: {
    Home
  },
  data() {
    return {
     todos : [
       { 
         id : 1,
         title : "titre 1",
         value : "1245887",
         isComplete : true,
       },
       {
         id : 2,
         title : "titre 2",
         value : "heheheh ehuiz",
         isComplete : false,
       },
       {
         id : 3,
         title : "titre 3",
         value : "test test",
         isComplete : true,
       }
     ]
    }
  }
}
</script>

<style>
  body{
    margin: 0;
    padding: 0;
    background: #e8e8e8;
  }
</style>
