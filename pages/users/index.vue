<template>
  <section>
    <input v-model="userID" type="text">
    <button @click="onLoadUser">
      Load User
    </button>
  </section>
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
