<template>
    <h1>Get input value</h1>
    <label for="java">Java</label>
    <input type="checkbox" value="java" id="java" v-model="technology">

    <label for="php">PHP</label>
    <input type="checkbox" value="php" id="php" v-model="technology">
 
    <label for="node">NodeJS</label>
    <input type="checkbox" value="node" id="node" v-model="technology">

    <br><br>

    <h3>Who I am</h3>

    <label for="student">student</label>
    <input type="radio" value="student" name="who" v-model="who">

    <label for="developer">developer</label>
    <input type="radio" value="developer" name="who" v-model="who">

    <h4>I am a: {{ who }}</h4>

    <h4>Selected Technology: {{ technology }}</h4>
</template>

<script>
    export default {
        name: 'MainHome',
        data() {
            return {
                technology: [], //to show more than one value
                who: null //to show only one value per time
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