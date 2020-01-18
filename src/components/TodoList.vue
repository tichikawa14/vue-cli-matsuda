<template>
  <ul>
    <li
      v-for="todo in todoList"
      :key="todo.id"
    >
      {{ todo.title }}
      {{ todo.content }}
    </li>
  </ul>
</template>

<script>
  export default {
    name: 'TodoList',
    data: function() {
      return {
        todoList: [
          { id: 1, title: "データ", content: "dsa" },
          { id: 2, title: "データ2", content: "dsa2" },
          { id: 3, title: "データ3", content: "dsa3" }
        ]
      }
    },
    props: {
      msg: String,
      description: String
    }
  }
</script>

<style scoped>
</style>