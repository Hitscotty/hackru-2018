<template>
  <div>
    <Header></Header>
    <div id="render-body" ref="render-body">
      <HomePage v-if="pages['home']"></HomePage>
      <DefriendPage v-if="pages['defriender']"></DefriendPage>
    </div>
  </div>
</template>

<script>
  import App from "./App.vue";

  import Header from "./sections/Header"
  import HomePage from "./sections/HomePage"
  import DefriendPage from "./sections/DefriendPage"

  export default {
    data() {
      return {
        pages: {
          home: false,
          defriender: true
        }
      }
    },
    components: {
      Header,
      HomePage,
      DefriendPage
    },
    methods: {
      toggle(page) {
        Object.keys(this.pages).forEach(key => {
          console.log(key);
          if (key === page) {
            this.pages[key] = true;
          } else {
            this.pages[key] = false;
          }
        })

      },
      initRouter() {
        const vm = this;
        this.$nextTick(() => {
          $("#pager").on("click", "a", function () {
            const page = $(this).data("page")
            vm.toggle(page);
          });
        })
      }
    },
    mounted() {
      this.initRouter();
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

  h1,
  h2 {
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
