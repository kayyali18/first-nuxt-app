<template>
  <div>
    <input v-model="pID" type="text">
    <button @click="routeUser">
      Click Me
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      pID: ''
    }
  },
  methods: {
    routeUser() {
      this.$router.push(`/products/${this.pID}`)
    }
  }
}
</script>
