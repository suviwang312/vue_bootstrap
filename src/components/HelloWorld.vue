<template>
  <div class="hello">
    <div class="container">
      <div class="row">
        <div class="col-sm">
          <div class="alert alert-primary" role="alert">
            A simple primary alert—check it out!
          </div>
          <div class="alert alert-secondary" role="alert">
            A simple secondary alert—check it out!
          </div>
          <div class="alert alert-success" role="alert">
            A simple success alert—check it out!
          </div>
          <div class="alert alert-danger" role="alert">
            A simple danger alert—check it out!
          </div>
        </div>
        <div class="col-sm">
          One of three columns
        </div>
        <div class="col-sm">
          One of three columns
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
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
