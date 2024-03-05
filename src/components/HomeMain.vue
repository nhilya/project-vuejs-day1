<template>
    <div>
        <h1>Pass data to child components</h1>
        <MyChild name = "sam" :user="user" get-data="GetData"/>
    </div>
</template>

<script>
     import MyChild from './MyChild.vue'
    export default {
        name: 'HomeMain',
        components: {
            MyChild
        },
        data() {
            return {
                user: {name: 'sam', email: 'sam@gmail.com'}
            }
        },
        methods: {
            getData() {
                console.warn("parent function called")
            }
        }
    }
</script>

<style scoped>
/* scoped: To only apply style for this component file only. */
    h1 {
        color: red;
    }
</style>