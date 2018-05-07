<template>
  <div id="app">
    <img width="25%" src="./assets/logo.png">
    <br>
    <a href="" @click.prevent="tampilanSekarang='Login'">login</a>
    <a href="" @click.prevent="tampilanSekarang='Signup'">signup</a>
    <component :is="tampilanSekarang"/>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import Login from "./components/Login";
import Signup from "./components/Signup";

export default {
  name: "App",
  data() {
    return {
      tampilanSekarang: "Signup"
    };
  },
  components: {
    HelloWorld,
    Login,
    Signup
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
a {
  background-color: black;
  color: white;
  display: inline-block;
  width: 100px;
  height: 40px;
  line-height: 40px;
  text-decoration: none;
  margin: 5px;
}
</style>
