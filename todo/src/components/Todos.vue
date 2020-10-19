<template>
  <div>
    <div v-for="t in todos" v-bind:key="t.id">
      <TodoItem v-bind:todo="t"/>
    </div>
  </div>
</template>

<script>

import TodoItem from './TodoItem.vue'

export default {
  name: "Todos",
  props: ["todos"],
  components: {
    TodoItem
  }
}
</script>

<style lang="stylus" scoped>

</style>