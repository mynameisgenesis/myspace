<template>
  <div id="nav" class="text-center">
    <router-link to="/">Home</router-link> |
    <router-link to="/browse">Browse</router-link> |
    <router-link to="/search">Search</router-link> |
    <router-link to="/invite">Invite</router-link> |
    <router-link to="/film">Film</router-link> |
    <router-link to="/mail">Mail</router-link> |
    <router-link to="/blog">Blog</router-link> |
    <router-link to="/favorites">Favorites</router-link> |
    <router-link to="/forum">Forum</router-link> |
    <router-link to="/groups">Groups</router-link> |
    <router-link to="/events">Events</router-link> |
    <router-link to="/videos">Videos</router-link> |
    <router-link to="/music">Music</router-link> |
    <router-link to="/comedy">Comedy</router-link> |
    <router-link to="/classified">Classified</router-link>
  </div>
</template>

<script>
export default {
  name: "PageNavigation",
};
</script>

<style>
#nav,
#nav > a {
  background-color: #5fa5f8;
  color: #000000;
}

#nav > a {
  text-decoration: none;
  color: #ffffff;
}
</style>
