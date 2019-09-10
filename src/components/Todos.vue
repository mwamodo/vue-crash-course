<template>
  <div>
    <div v-bind:key="todo.id" v-for="todo in todos">
      <!-- <h3>{{ todo.title }}</h3> -->
      <TodoItem v-bind:todo="todo" />
    </div>
  </div>
</template>

<script>
import TodoItem from "@/components/TodoItem";

export default {
  name: "Todos",
  props: ["todos"],
  components: {
    TodoItem
  }
};
</script>

<style scoped>
</style>