<template>
  <div id="app">
    <div class="conatiner">
      <product-list />
    </div>
  </div>
</template>

<script>
import ProductList from './components/ProductList'

export default {
  name: 'App',
  components: {
    ProductList
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
}
</style>
