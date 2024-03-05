<template>
    <div>
        <h1>Task 4 Evening Assignment</h1>
        <ul>
            <!-- Use v-for to render each item in the items array as a list item -->
            <li v-for="(item, index) in items" :key="index" @click="handleItemClick(item)">
                {{ item }}
            </li>
        </ul>
    </div>
</template>
  
<script>
export default {
    name: 'ItemList',
    data() {
        return {
            // Array of items
            items: ['Item 1', 'Item 2', 'Item 3', 'Item 4']
        };
    },
    methods: {
        // Method to handle click event on an item
        handleItemClick(item) {
            alert(`You clicked on ${item}`);
        }
    }
}
</script>
  
<style>
/* Style your list items here */
li {
    cursor: pointer;
    /* Change cursor to indicate clickable items */
    margin: 5px 0;
    /* Add some spacing between items */
}
</style>
  