<template>
  <div id="app">
    <div class="jumbotron">
      <div class="container">
        <h1 class="display-3">{{ msg }}</h1>
        <p>Enter the number, avoid Awkward Conversations Now!</p>
        <p><a class="btn btn-primary btn-lg" href="#" role="button" @click="learnBtn">Learn more &raquo;</a></p>
      </div>
    </div>
    
<div class="container">
      <!-- Example row of columns -->
      <div class="row">
        <div class="col-md-4">
          <h2>What</h2>
          <p>Defriend Me is SPA that helps you avoid conversations . </p>
          <p><a class="btn btn-secondary" href="#" role="button" @click="whyBtn">View details &raquo;</a></p>
        </div>
        <div class="col-md-4">
          <h2>How</h2>
          <p>We allow our software to contact the person you want to lose contact with. </p>
          <p><a class="btn btn-secondary" href="#" role="button" @click="howBtn" >View details &raquo;</a></p>
       </div>
        <div class="col-md-4">
          <h2>Why</h2>
          <p>We Felt it was neccesary .</p>
          <p><a class="btn btn-secondary" href="#" role="button" @click="whyBtn" >View details &raquo;</a></p>
        </div>
      </div>

      <hr>

      <footer>
        <p>&copy; Company 2017</p>
      </footer>
    </div> <!-- /container -->
    
    <h2>Ecosystem</h2>
    <ul>
      <li><a href="http://router.vuejs.org/" target="_blank">vue-router</a></li>
      <li><a href="http://vuex.vuejs.org/" target="_blank">vuex</a></li>
      <li><a href="http://vue-loader.vuejs.org/" target="_blank">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank">awesome-vue</a></li>
    </ul>
  </div>
</template>

<script>
import Content from "./sections/Content"
import Footer from "./sections/Footer"

export default {
  name: 'app',
  data () {
    return {
      msg: 'Defriend Me'
    }
  },
  methods:{
    learnBtn(){
    swal("Learn More", "Life is hard enough as it is. Avoid awkward conversations with shitty significant others, creeps and general miscreants.");
  },
    whatBtn(){
    swal("What", "We make the call so you dont have to.");
  },
    howBtn(){
    swal("How", "Magic,love and social anxiety");
  },
    whyBtn(){
    swal("Why?", "Cause reasons");
  }
  },
  components: {
    Content,
    Footer
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
