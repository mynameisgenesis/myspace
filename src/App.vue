<template>
  <div id="app" class="container">
    <page-header />
    <router-view></router-view>
  </div>
</template>

<script>
import PageHeader from "./components/PageHeader.vue";
export default {
  components: { PageHeader },
  name: "App",
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
