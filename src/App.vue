<template>
  <div id="app">
    <MoblePage v-if="1"></MoblePage>
    <PCPage></PCPage>
  </div>
</template>

<script>
import MoblePage from './components/mobile/index.vue';
import PCPage from './components/pc/index.vue';
export default {
  name: 'app',
  components: {
    MoblePage,
    PCPage
  },
  data () {
    return {
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

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
