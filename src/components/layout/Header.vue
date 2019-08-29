<template>
  <header class="header">
    <h1>TodoList</h1>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">&nbsp;About</router-link>
    </div>
  </header>
</template>

<script>
  export default {
    name: "Header"
  }
</script>

<style scoped>
  .header {
    background: #333;
    color: #fff;
    text-align: center;
    padding: 10px;
  }

  .header a {
    color: #fff;
    padding-right: 5px;
    text-decoration-line: none;
    cursor: pointer;
  }
</style>