<template>
    <div>
        <input type="checkbox" v-on:change="selected">
       {{ todo.title }}
    </div>
</template>
<script>

export default {
    name : "TodoItem",
    props : ["todo"],
    methods : {
        selected(){
           
            this.todo.isComplete = !this.todo.isComplete;
          
        }
    }
}
</script>
<style scoped>
    
</style>