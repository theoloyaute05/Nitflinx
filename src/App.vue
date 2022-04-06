<template>
  <NavBar/>
  <NowplayingMovies/>
  <PopularMovies/>
  <PopularSeries/>
  <TopratedMovies/>
  <TopratedSeries/>
  <UpcomingMovies/>
</template>

<script>
import NavBar from './components/Navbar.vue'
import NowplayingMovies from './components/NowplayingMovies.vue'
import PopularMovies from './components/PopularMovies.vue'
import PopularSeries from './components/PopularSeries.vue'
import TopratedMovies from './components/TopratedMovies.vue'
import TopratedSeries from './components/TopratedSeries.vue'
import UpcomingMovies from './components/UpcomingMovies.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    NowplayingMovies,
    PopularMovies,
    PopularSeries,
    TopratedMovies,
    TopratedSeries,
    UpcomingMovies
  }
}
</script>

<style>
#app {
  
}
</style>
