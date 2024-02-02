<template>
<router-link to="/">홈으로</router-link>
<div>
    <h5>{{blog[$route.params.id].title}}</h5>
    <p>{{blog[$route.params.id].content}}</p>
    <p>{{blog[$route.params.id].date}}</p>
</div>
</template>

<script>
export default {
    props : {
        blog : Array
    }
}
</script>

<style>

</style>