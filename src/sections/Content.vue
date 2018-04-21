<template>
  <div class="col-6 card px-4 py-3">
    <div class="card-body">
      <form class="ui form">
        <div class="field inline">
          <label> Phone #</label>
          <input name="phone" placeholder="(xxx) - xxx - xxxx" />
        </div>
        <div class="two fields inline">
          <label> Name </label>
          <div class="field inline">
            <input name="first" />
          </div>
          <div class="field inline">
            <input name="last" />
          </div>
        </div>
        <div class="field inline">
          <label for="embedpollfileinput" class="ui huge green floated button" @click="phoneM">
            <i class="ui upload icon"></i>
            Upload Audio
          </label>
        </div>
        <button class="ui green button"> send </button>
      </form>
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
<style>
  .inputfile {
    width: 0.1px;
    height: 0.1px;
    opacity: 0;
    overflow: hidden;
    position: absolute;
    z-index: -1;
  }

</style>
