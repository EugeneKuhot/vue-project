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
  methods: {
    changeName() {
      debugger
      return this.carName = 'df'
    }
  },
  data () {
    return {
      title: 'Welcome',
      carName: 'Audi',
      carYear: 2000
    }
  },
  beforeMount() {
    this.$on('nameChanged', this.changeName())
  }
}
</script>

<style>
</style>
