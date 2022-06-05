<template>
  <h2 v-for="(name, index) in names" :key="name">{{ index }} {{ name }}</h2>
  <h2 v-for="name in fullNames" :key="name.first">{{ name.first }} {{ name.last }}</h2>
  <div v-for="actor in actors" :key="actor.name">
    <h2>{{ actor.name}}</h2>
    <h2 v-for="movie in actor.movies" :key="movie">{{ movie }}</h2>
  </div>

  <h2 v-for="(info, key, index) in myInfo" :key="info">{{ index }} : {{ key }} {{ info }}</h2>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      names: ['Bruce', 'Clark', 'Diana'],
      fullNames: [
        { first: 'Iris', last: 'DeLora'},
        { first: 'Anita', last: 'Duong'},
        { first: 'Jess', last: 'Tham'},
      ],
      actors: [
        {
          name: 'Christian Bale',
          movies: ['Batman', 'American Psycho'],
        },
        {
          name: 'Di Caprio',
          movies: ['Titanic', 'Inception'],
        },
      ],
      myInfo: {
        name: 'Iris DeLora',
        course: 'Vue 3',
        age: 22
      },
    }
  },
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
