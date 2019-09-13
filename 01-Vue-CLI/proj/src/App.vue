<template>
  <div id="app">
    <header>
      <span>Vue.js PWA</span>
    </header>
    <main>
      <!-- <img src="./assets/logo.png" alt="Vue.js PWA"> -->
      <img src="./assets/lololo.png" alt="Vue.js PWA">
      <div class="message-test">
        <p>[[[[testmsg]]]]</p>
        <p>{{ message }}</p>
        <button v-on:click="reverseMessage">Reverse Message</button>
      </div>
      <router-view></router-view>
    </main>
  </div>
</template>

<script>
export default {[
  {
    name: 'app'
  },
  {
    name: '#app',
    data: {
      message: 'Hello Vue!'
    },
    methods: {
      reverseMessage: function () {
        this.message = this.message.split('').reverse().join('')
      }
    }
  }
]}
</script>

<style>
body {
  margin: 0;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

main {
  text-align: center;
  margin-top: 40px;
}

header {
  margin: 0;
  height: 56px;
  padding: 0 16px 0 24px;
  background-color: #35495E;
  color: #ffffff;
}

header span {
  display: block;
  position: relative;
  font-size: 20px;
  line-height: 1;
  letter-spacing: .02em;
  font-weight: 400;
  box-sizing: border-box;
  padding-top: 16px;
}
</style>
