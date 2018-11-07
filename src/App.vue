<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <PizzaBooking/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import TicketBooking from './components/TicketBooking.vue'
import PizzaBooking from './components/PizzaBooking.vue'

export default {
  name: 'app',
  components: {
    TicketBooking,
    PizzaBooking
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
</style>
