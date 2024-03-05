<template>
    <h1>{{ text }}</h1>
    <div v-html="tag">
    
    </div>
</template>

<script>
    export default {
        name: 'MainHome',
        data() {
            return {
                text: "sam",
                tag: "<h1>alex</h1>"
            }
        }
    }
</script>