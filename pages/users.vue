<template>
  <div>
    <h1>Hi user.</h1>
    <input type="text" v-model="userId">
    <button @click="onLoadUser">Load user</button>
    <nuxt-child></nuxt-child>
  </div>
</template>

<script>
export default {
  name: "users",
  data() {
    return {
      userId: ''
    }
  },
  methods: {
    onLoadUser() {
      this.$router.push('/users/' + this.userId);
    }
  },
  layout: 'users'
}
</script>

<style scoped>

</style>
