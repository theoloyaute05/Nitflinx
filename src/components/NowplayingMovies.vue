<template>
    <div class="title">Current Movies :</div>
    <div class="align-movie">
        <div :style = "'background-image: url(https://image.tmdb.org/t/p/original/' + movie.poster_path + ');'" class="movie" v-for="movie in post" :key="movie.id"></div>
    </div>
</template>

<script>
export default {
  name: 'NowplayingMovies',
  data: function() {
    return {post: {}}
  },

  methods: {
    async getData() {
      try {
        let response = await fetch('https://api.themoviedb.org/3/movie/now_playing?api_key=166a3de7cb9e6eb15d106b33466368b0&language=en-US&page=1');
        response = await response.json();
        this.post = response.results;
        console.log(this.post);
      } catch (error) {
        console.log(error);
      }
    }
  },

  created() {
    this.getData();
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Hubballi&family=Raleway:ital,wght@1,100&family=Roboto&display=swap');

  .title {
    color: #fff;
    font-size: 1.8em;
    font-family: 'Roboto', sans-serif;
    margin-top: 10vh;
    margin-bottom: -4vh;
  }

  .align-movie {
    display: flex;
    flex-direction: row;
    width: 300vw;
    height: 50vh;
  }

  .movie {
    background: center / contain no-repeat;
    width: 13vw;
    height: 50vh;
    color: #fff;
    margin: 1vw;
  }
</style>