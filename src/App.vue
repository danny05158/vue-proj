<template>
  <div id="app">
    <Icons />
  </div>
</template>

<script>
import Icons from './components/Icons.vue'

export default {
  name: 'App',
  components: {
    Icons
  }
}
</script>

<style>

body {
   background-image: linear-gradient(to bottom, #ff8a00, #e52e71);
   height: 100vh;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

/* above 1000 show 6 coumns */
@media (min-width: 1000px){

   .dragArea{
     margin: 0 100px !important;
     justify-content: space-between;
   }

}

/* between 999 - 500 show 4 colums */
@media (max-width: 999px){

  .dragArea{
    flex-wrap: wrap;
    justify-content: center;
    margin: 0 30px !important;
  }

    .icon-container{
    margin: 3px 2px !important;
    flex-basis: 20%;
   }
}

/* below 500 show 2 colums */
@media (max-width: 499px){

  .icon-container{
    flex-basis: 33% !important;
  }
}


</style>
