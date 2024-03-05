<template>
    <div>
        <h1> {{ name }}</h1>
        <h2> {{ user.name }}</h2>
        <button @click="getData">Call Function</button>
    </div>
</template>

<script>
    import MyChild from './MyChild.vue'
    export default {
        name: 'MyChild',
        props: {
            name: Object,
            user: String,
            getData: Function
        }
    }
</script>


<style>

</style>