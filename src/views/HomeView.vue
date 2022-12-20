<template>
  <div id="homepage" class="row">
    <h5>Jessica <b>Genesis Belmonte</b></h5>
    <div class="col d-inline-flex">
      <img id="profile-pic" class="d-inline" src="../assets/profile-pic.jpeg" />
      <div class="px-2 w-25">
        <small>"Don't cry because it's over smile because it happened."</small>
        <br /><br />
        <small class="p-4">
          Female<br />30 years old<br />Pueblo West<br />COLORADO<br />United
          States
        </small>
        <br /><br />
        <small class="profile-pic-text"> Last Login:<br /> </small>
        <small>{{ currentDate }}</small>
      </div>
    </div>
    <div class="col"></div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  computed: {
    currentDate() {
      var currentDateWithFormat = new Date()
        .toJSON()
        .slice(0, 10)
        .replace(/-/g, "/");
      return currentDateWithFormat.toString();
    },
  },
};
</script>

<style>
#profile-pic,
#profile-pic-text {
  max-height: 350px;
}
</style>
