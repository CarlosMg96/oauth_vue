<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link>|
      <router-link to="/about">About</router-link>|
      <router-link v-if="$auth.isAuthenticated" to="/profile"
        >Profile</router-link
      >
    </div>
    <router-view />
  </div>
</template>

<script>
export default {};
</script>

<style>
#app {
  font-family: Arial, sans-serif;
  color: #333;
  background-color: #f5f5f5;
}

#nav {
  background-color: #24292e;
  padding: 20px;
  color: #fff;
}

#nav a {
  color: #fff;
  text-decoration: none;
  margin-right: 10px;
}

#nav a:hover {
  color: #ccc;
}
</style>