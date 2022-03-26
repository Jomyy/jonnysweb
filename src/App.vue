<template>
  <nav>
    <p>PRODBYJONNY</p>
    <router-link to="/">HOME</router-link> | <router-link to="/about">ABOUT</router-link>
  </nav>

  <router-view />
</template>

<style>
@font-face {
  font-family: "FuturaPT";
  src: url("./assets/FuturaPTHeavy.otf") format("opentype");
  font-style: normal;
}
#app {
  font-family: FuturaPT, FuturaPT;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: black;
  padding: 0px;
  margin: 0px;
}
body {
  margin: 0px;
  padding: 0px;
  background-color: #f3f3f3;
}
@media screen and (max-width: 500px) {
  nav p {
    display: none;
  }
}
nav {
  position: fixed;
  background-color: #f3f3f3a6;

  -webkit-backdrop-filter: blur(40px);
  backdrop-filter: blur(40px);
  margin: 7px;
  color: black;
  padding: 0px;
  margin: 0px;
  height: 60px;
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 10;
}
nav p {
  position: absolute;
  left: 20px;
}
nav a {
  font-weight: bold;
  color: blue;
  padding-left: 10px;
  padding-right: 10px;
}

nav a.router-link-exact-active {
  color: black;
}
</style>
