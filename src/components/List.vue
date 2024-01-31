<template>
  <div>
    <h5>{{b.title}}</h5>
    <p>{{b.content}}</p>
    <p>{{b.date}}</p>
    <p></p>
  </div>
</template>

<script>
export default {
    props : {
        b : Object
    }
}
</script>

<style>

</style>