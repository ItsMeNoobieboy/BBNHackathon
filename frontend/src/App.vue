<template>
  <nav>
    <router-link to="/">Map</router-link> |
    <router-link to="/plow">Plow</router-link>
  </nav>
  <router-view />
</template>

<script src>
window.ws = new WebSocket('ws://localhost:3000')
</script>

<style>
#app {
  font-family: Avenir, Hezlvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* remove overflow */
  overflow: hidden;
}
body, html, #app {
  height: 100%;
  margin: 0px;
  padding: 0px;
}
nav {
  padding: 0.75rem;
  background-color:  rgb(184,216,237);
  font-size: 1rem;
}
nav a {
  color: rgb(13,39,92);
}
</style>