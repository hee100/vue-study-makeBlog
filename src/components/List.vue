<template>
  <div v-for="(b, i) in blog" :key=i>
    <h5 @click="$router.push('detail/' + i)">{{b.title}}</h5>
    <p>{{b.content}}</p>
    <p>{{b.date}}</p>
    <p></p>
  </div>
</template>

<script>
export default {
    props : {
        blog : Object
    }
}
</script>

<style>

</style>