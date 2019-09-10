<template>
  <div class="home">
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
// @ is an alias to /src
import Todos from "@/components/Todos";

export default {
  name: "home",
  components: {
    Todos
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          title: "Todo One",
          completed: false
        },
        {
          id: 2,
          title: "Todo Two",
          completed: true
        },
        {
          id: 3,
          title: "Todo Three",
          completed: false
        }
      ]
    };
  }
};
</script>
