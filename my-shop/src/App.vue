<template>
  <div id="app">
    <ProductCard
      name="Єгипетський хрест Анх"
      description="Символ життя в стародавньому Єгипті, виготовлений із бронзи."
      image="https://i.pinimg.com/736x/99/67/2d/99672d7447d2b08562e691a8fb27b984.jpg"
      :price="410"
    />
  </div>
</template>

<script>
import ProductCard from './components/ProductCard.vue'

export default {
  name: 'App',
  components: {
    ProductCard
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
