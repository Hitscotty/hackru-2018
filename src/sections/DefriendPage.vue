<template>
  <div class="container">
    <div class="heading text-center py-4">
      <p class="h2">
        Our experts love to answer questions.
        <br> Fill out the form below.
      </p>
    </div>
    <div class="row justify-content-md-center">
      <div class="col-6">
        <div class="card">
          <div class="uk-grid">
            <div class="text-center">
              <form class="ui form">
                <div class="field inline">
                  <label>
                    Phone #
                  </label>
                  <input name="phone" placeholder="(xxx) xxx xxxx" />
                </div>
                <div class="field inline">
                  <label for="embedpollfileinput" class="ui huge green floated button" @click="phoneM">
                    <i class="ui upload icon"></i>
                    Upload Audio
                  </label>
                </div>
                <button class="ui green button float-right"> send </button>

              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    methods: {
      phoneM() {
        swal("Wait", "Why not just call them then?");

      }
    }
  }

</script>
