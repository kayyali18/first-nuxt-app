<template>
  <p>Please enter ID</p>
</template>


<script>
export default {
  data() {
    return {
      userID: ''
    }
  },
  methods: {
    onLoadUser() {
      this.$router.push(`/users/${this.userID}`)
    }
  }
}
</script>
