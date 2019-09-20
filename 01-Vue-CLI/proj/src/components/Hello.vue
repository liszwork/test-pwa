<template>
  <div>
    <div class="hello">
      <h1>{{ msg }}</h1>
      <p>== {{ fugamsg }} ==</p>
      <hr />
      <p>!! {{ message }} ??</p>
      <button v-on:click="reverseMessage">Reverse Message</button>
    </div>
    <div class="hoge">
      <p>-- {{ hogemsg }} --</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'sample projectttttttt',
      fugamsg: 'hugahuga',
      message: 'Hello vue.'
    }
  },
  methods: {
    reverseMessage: function () {
      this.message = this.message.split('').reverse().join('')
    }
  }
}

// export { hello, hoge }
// function hello() {
//   return {
//     msg: 'sample projectttttttt',
//     fugamsg: 'hugahuga'
//   }
// }
// function hoge() {
//   return 'hogehoge'
// }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
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
  color: #35495E;
}
</style>
