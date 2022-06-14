<template>
  <product-list-one v-bind:products="products"></product-list-one>
  <product-list-two v-bind:products="products"></product-list-two>
</template>

<script>
import ProductListOne from './components/ProductItemsOne.vue'
import ProductListTwo from './components/ProductItemsTwo.vue'

export default {
  name: 'App',
  components: {
    'product-list-one': ProductListOne,
    'product-list-two': ProductListTwo,
  },

  data() {
    return {
      products: [
        {name: 'Pen', price: 20},
        {name: 'Pencil', price: 15},
        {name: 'Erase pen', price: 80},
        {name: 'Ruler', price: 15},
        {name: 'pencil case', price: 100},
        {name: 'Crayon', price: 120},
        {name: 'chalk', price: 10},
      ]     
    }
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
