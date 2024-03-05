<template>
    <div>
        <h1>Get 3 input value</h1>
        <input type="text" placeholder="Enter your name" v-model="name">
        <br><br>
        <input type="email" placeholder="Enter your email..." v-model="email">
        <br><br>
        <input type="password" placeholder="Enter your password" v-model="password">
        <br><br>
        <button v-on:click="getData()" type="button">Get value</button>
        <br><br>
    <!-- Table to display the data -->
    <table v-if="submitted">
      <thead>
        <tr>
          <th>Name</th>
          <th>Email</th>
          <th>Password</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>{{ name }}</td>
          <td>{{ email }}</td>
          <td>{{ password }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
    export default {
        name: 'TaskOne',
        data() {
            return {
                name: null,
                email: null,
                password: null,
                submitted: false // Flag to show/hide the table
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
th, td {
    border: 1px solid black;
    padding: 8px;
    text-align: left;
}
</style> 