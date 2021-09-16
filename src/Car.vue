<template>
  <div>
    <p>Name: {{ carName }}</p>
    <p>Year: {{ carYear }}</p>
    <button @click="changeName">Change name</button>
  </div>
</template>

<script>
export default {
  name: 'Car',
  props: {
    carName: String,
    carYear: Number
  },
  methods: {
    changeName() {
      this.carName = 'carName'
      this.$emit('nameChanged', this.carName)
    }
  },
  data() {
    return {
    }
  }
}

</script>

<style>

</style>
