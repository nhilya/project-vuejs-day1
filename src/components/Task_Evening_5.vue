<template>
    <div id="app">
        <h1>Task 5 Evening Assignment</h1>
        <h3>Counter: {{ counter }}</h3>
        <button @click="increment">Increment</button>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            counter: 0
        }
    },
    watch: {
        counter(newValue, oldValue) {
            console.log('Counter changed from', oldValue, 'to', newValue)
        }
    },
    methods: {
        increment() {
            this.counter++
        }
    }
}
</script>