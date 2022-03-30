<template>
  <div id="nav">
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
    <router-link to="/different">Difference</router-link>
    <router-link to="/nps">NpsSystems</router-link>
  </div>
  <router-view />
</template>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  /* overflow: auto; */
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-image: url("./assets/bg-mobile2.png");
  background-repeat: no-repeat;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

@media only screen and (min-width: 700px) {
  #app {
    background-image: url("./assets/bg-desktop.png");
    background-repeat: no-repeat;
    background-position-x: center;
    background-position-y: right;
  }
}
</style>
