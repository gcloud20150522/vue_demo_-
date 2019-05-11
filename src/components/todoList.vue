<template>
  <ul class="todo-main">
    <TodoItem v-for="(todo,index) in todos" :todo="todo" :key="index" :index="index"/>
  </ul>
</template>

<script>
  import TodoItem from "./todoItem"

  export default {
    props:{
      todos:Array,
      
    },
    components:{TodoItem}
  }
</script>

<style>
/*main*/
.todo-main {
  margin-left: 0px;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding: 0px;
}

.todo-empty {
  height: 40px;
  line-height: 40px;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding-left: 5px;
  margin-top: 10px;
}

</style>
