<template>
    <div>
        <h1>{{ greeting }}</h1>
    </div>
</template>
  
<script>
export default {
    name: 'GreetingsMessage',
    data() {
        return {
            greeting: ""
        };
    },
    created() {
        this.updateGreeting();
        setInterval(this.updateGreeting, 60000); // Update greeting every minute
    },
    methods: {
        updateGreeting() {
            const currentHour = new Date().getHours();
            if (currentHour >= 6 && currentHour < 12) {
                this.greeting = "Good morning";
            } else if (currentHour >= 12 && currentHour < 18) {
                this.greeting = "Good afternoon";
            } else if (currentHour >= 18 && currentHour < 24) {
                this.greeting = "Good evening";
            } else {
                this.greeting = "Good night";
            }
        }
    }
};
</script>
   