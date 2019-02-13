<template>
  <h1>A Single User with ID: {{ $route.params.id }} and the object of {{ info }}</h1>
</template>

<script>
export default {
  data() {
    return {
      info: {}
    }
  },
  validate(data) {
    return parseInt(data.params.id) === 1
  }
}
</script>
