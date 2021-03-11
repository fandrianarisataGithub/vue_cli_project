<template>
    <div class="mydiv">
        <div v-bind:key="todo.id" v-for="todo in todos">
           <TodoItem v-bind:todo="todo"/>
        </div>
    </div>
</template>
<script>
import TodoItem from '@/components/TodoItem'
export default {
    name : "Home",
    props : ["todos"],
    components : {
        TodoItem,
    }
}
</script>
<style scoped>
    
</style>