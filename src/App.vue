<template>
  <div id="app">
    <h1>{{ title }}</h1>
    <Car :carName="carName" :carYear="carYear"/>
  </div>
</template>

<script>
import Car from "./Car";

export default {
  name: 'app',
  components: {
    Car
  },
  data () {
    return {
      title: 'Welcome',
      carName: 'Audi',
      carYear: 2000
    }
  }
}
</script>

<style>
</style>
