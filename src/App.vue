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
  computed: {
    backgroundImage() {
      switch (this.$route.name) {
        case "Home":
          return null;
        case "Contact":
          return require("./assets/win95/clouds2.jpg");
      }
      return null;
    },
  },
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
