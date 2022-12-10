<template>
  <div id="header" class="row">
    <div id="search" class="row g-0 text-center">
      <div class="col-6">
        <input
          class="w-100"
          type="search"
          placeholder="Search..."
          aria-label="Search"
        />
      </div>
      <div class="col-2">
        <select name="search-select" id="search-select" class="h-100">
          <option value="myspace">MySpace</option>
        </select>
      </div>
      <div class="col-2">
        <button class="h-100 w-100">Search</button>
      </div>
      <div id="google-logo-container" class="col-2">
        <img
          id="google-logo"
          src="../assets/powered-by-google.png"
          alt="Powered by Google"
          srcset=""
        />
      </div>
    </div>

    <page-navigation />
  </div>
</template>

<script>
import PageNavigation from "./PageNavigation.vue";
export default {
  name: "PageHeader",
  components: {
    PageNavigation,
  },
  data() {
    return {};
  },
};
</script>

<style scoped>
#search {
  background-color: #1c4ed8;
  padding: 20px 50px 20px 50px;
}
#search-select {
  width: 90%;
}

#google-logo {
  width: 100px;
}
</style>
