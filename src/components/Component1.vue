<template>
  <div class="hello">
      {{count}}
      {{name}}
      <button @click="increment">+</button>
      <div>
        <input type="text">
        <button>Add names</button>
      </div>
  </div>
</template>

<script>
export default {
name: 'Component1',
props: {
msg: String
},
computed: {
    count() {
        return this.$store.state.count
    }
},
methods: {
    increment() {
      this.$store.commit("increment");
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
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
