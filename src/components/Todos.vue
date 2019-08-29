<template>
  <div>
    <div v-for="todo in todos" :key="todo.id">
      <todo-item :todo="todo" @del-todo="$emit('del-todo', todo.id)"></todo-item>
    </div>
  </div>
</template>

<script>
  import TodoItem from './TodoItem'

  export default {
    name: "Todos",

    components: {
      TodoItem
    },

    props: ["todos"]
  }
</script>

<style scoped>

</style>