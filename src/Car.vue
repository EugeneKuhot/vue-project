<template>
  <div>
    <p>Name: {{ carName }}</p>
    <p>Year: {{ carYear }}</p>
  </div>
</template>

<script>
export default {
  name: 'Car',
  props: {
    carName: String,
    carYear: Number
  },
  data() {
    return {
    }
  }
}

</script>

<style>

</style>
