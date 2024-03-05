<template>
    <div>
        <h1>For loop in Vue</h1>
        <ul>
            <li v-for="item in technology" :key="item">
                {{ item }}
            </li>
        </ul>
        <br>
        <ul>
            <li v-for="item in user" :key="item">
                Name: {{ item.name }} and Email is : {{ item.email }}
            </li>
        </ul>
    </div> 
</template>

<script>
export default {
    name: 'ForLoop',
    data() {
        return {
            technology: ['java', 'php', 'vuejs'],
            // array of object
            user: [
                {
                    name: 'sam',
                    email: 'sam@gmail.com'
                },
                {
                    name: 'alex',
                    email: 'alex@gmail.com'
                },
                {
                    name: 'bruce',
                    email: 'bruce@gmail.com'
                }
            ]
        }
    },
    methods: {
        getData() {
            this.submitted = true; // Show the table when data is submitted
            console.warn("values: ", this.name, this.email, this.password);
        }
    }
}
</script>

<style>
table {
    width: 100%;
    border-collapse: collapse;
}

th,
td {
    border: 1px solid black;
    padding: 8px;
    text-align: left;
}
</style>