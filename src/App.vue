<template>
<nav class="navbar bg-body-tertiary">
  <div class="container-fluid">
    <span class="navbar-brand mb-0 h1">Vuelog</span>
  </div>
</nav>
<!-- <div v-for="(b, i) in blog" :key=i>
  <List :b="blog[i]"/>
</div> -->
<List :b="blog[i]" v-for="(b, i) in blog" :key=i />

<Room @openModal="checkModal = true; roomNum = $event" :oneRoom="oneRooms[i]"
   v-for="(oneRoom, i) in oneRooms" :key="i"/>

</template>

<script>
import List from './components/List.vue'
import blog from './assets/blog'

export default {
  name: 'App',
  data() {
    return {
      blog : blog
    }
  },
  components: {
    List : List,
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
