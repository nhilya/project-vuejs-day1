<template>
  <HelloWorld msg="Welcome to our Vue App"/>
  <MainHome/>
  <TaskOne/>
  <Arguments/>
  <GreetingsMessage/>
  <Task_Evening_4/>
  <Task_Evening_5/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MainHome from './components/MainHome.vue'
import TaskOne from './components/TaskOne.vue'
import Arguments from './components/Arguments.vue'
import GreetingsMessage from './components/GreetingsMessage.vue'
import Task_Evening_4 from './components/Task_Evening_4.vue'
import Task_Evening_5 from './components/Task_Evening_5.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    MainHome,
    TaskOne,
    Arguments,
    GreetingsMessage,
    Task_Evening_4,
    Task_Evening_5
  }
}
</script>

<style>

</style>
 