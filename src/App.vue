<template>
<nav class="navbar bg-body-tertiary">
  <div class="container-fluid">
    <span class="navbar-brand mb-0 h1">Vuelog</span>
  </div>
</nav>

<div class="mt-3">
  <router-view :blog="blog"></router-view>
</div>
</template>

<script>
import blog from './assets/blog'

export default {
  name: 'App',
  data() {
    return {
      blog : blog
    }
  },
  components: { 

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
