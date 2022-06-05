<template>
<!-- Can't use arrow function in method & I don't know why-->
  <h2> Add method: {{ add(2, 3, 4)}}</h2>
  <h2> Suctract method: {{ subtract(3, 4)}}</h2>
  <h2> Multiply by {{ multyply(23)}}</h2>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      baseMultyply: 5,
    } 
  },

  methods: {
      add(a, b, c) {
        return a+b+c
      },
      subtract(a, b) {
        return a-b
      },
      multyply(num) {
        return num * this.baseMultyply
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
