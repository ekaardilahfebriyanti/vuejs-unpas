<template>
  <div class="signup">
    <h1>Sign Up</h1>
    <input type="text" placeholder="username"><br>
    <input type="password" placeholder="password"><br>
    <input type="password" placeholder="confirm password"><br>
    <button>SIGN UP</button>
  </div>
</template>

<script>
export default {
  name: "Signup",
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
