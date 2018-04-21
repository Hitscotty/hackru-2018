<template>
  <div id="app" class="container">
  <div class="row">
  <div class="col">
    <Header></Header>
    </div>
  </div>
   <div class="row justify-content-md-center">
     <Content></Content>
  </div>
   <div class="row">
      <div class="col">

     <Footer></Footer>
     </div>
  </div>
  </div>
</template>

<script>
import Content from "./sections/Content"
import Footer from "./sections/Footer"

export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
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
