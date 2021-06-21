<template>
  <div id='app'>
    <List title='Todos'/>
    <List title='Groceries'/>
  </div>
</template>

<script>
import List from './components/list';

export default {
  name: 'App',
  components: {
    List,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  display: flex;
  justify-content: space-around;
}
</style>
