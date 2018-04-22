<template>
  <section>
    <div class="jumbotron">
      <div class="container">
        <h1 class="display-3">{{ msg }}</h1>
        <p>Enter the number, avoid Awkward Conversations Now!</p>
        <p>
          <a class="btn btn-primary btn-lg" href="#" role="button" @click="learnBtn">Learn more &raquo;</a>
        </p>
      </div>
    </div>

    <div class="container">
      <div class="row">
        <div class="col-md-4">
          <h2>What</h2>
          <p>Defriend Me is SPA that helps you avoid conversations . </p>
          <p>
            <a class="btn btn-secondary" href="#" role="button" @click="whyBtn">View details &raquo;</a>
          </p>
        </div>
        <div class="col-md-4">
          <h2>How</h2>
          <p>We allow our software to contact the person you want to lose contact with. </p>
          <p>
            <a class="btn btn-secondary" href="#" role="button" @click="howBtn">View details &raquo;</a>
          </p>
        </div>
        <div class="col-md-4">
          <h2>Why</h2>
          <p>We Felt it was neccesary .</p>
          <p>
            <a class="btn btn-secondary" href="#" role="button" @click="whyBtn">View details &raquo;</a>
          </p>
        </div>
      </div>
      <hr>
    </div>
  </section>
</template>
<script>
  export default {
    name: 'app',
    data() {
      return {
        msg: 'Defriend Me'
      }
    },
    methods: {
      learnBtn() {
        swal("Learn More",
          "Life is hard enough as it is. Avoid awkward conversations with shitty significant others, creeps and general miscreants."
        );
      },
      whatBtn() {
        swal("What", "We make the call so you dont have to.");
      },
      howBtn() {
        swal("How", "Magic,love and social anxiety");
      },
      whyBtn() {
        swal("Why?", "Cause reasons");
      }
    }
  }

</script>
