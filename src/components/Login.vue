<template>
  <div class="login">
    <h1>LOGIN</h1>
    <input type="text" placeholder="username"><br>
    <input type="password" placeholder="password"><br>
    <button>LOGIN</button>
    <a href="">facebook</a>
  </div>
</template>

<script>
export default {
  name: "Login",
  data() {
    return {};
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
