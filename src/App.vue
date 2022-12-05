<template>
  <div id="app" class="container">
    <page-header />
    <section id="main-content">
      <router-view></router-view>
    </section>
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
#main-content {
  padding-top: 1em;
  padding-bottom: 1em;
}
</style>
