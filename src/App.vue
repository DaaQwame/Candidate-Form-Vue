<template>
  <nav>
    <router-link class="dip" to="/">Register</router-link>
    <router-link class="dip" to="/login">Login</router-link>
    <router-link class="dip" to="/candidates">All Candidate Details</router-link>
    <hr class="bar">
  </nav>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}
.dip{
   display: inline-block;
}
.bar{
  background-color: black;
  border: 1.5px solid black;
}
nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
  display: inline-block;
  padding: 0px 50px;
  text-transform: uppercase;
  padding-top: -6%;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
