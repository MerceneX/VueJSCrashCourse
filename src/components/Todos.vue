<template>
    <div>
        <div v-bind:key="todo.id" v-for="todo in todos">
            <ToDoItem/>
        </div>
    </div>
</template>

<script>
import ToDoItem from "./ToDoItem.vue";

export default {
    name:"Todos",
    components: {
        ToDoItem
        },
    props: ["todos"]
}
</script>

<style scoped>

</style>
