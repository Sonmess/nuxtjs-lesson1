<template>
  <p>Please enter an ID for user to load</p>
</template>

<script>
export default {
  name: "index",
  data() {
    return {
      userId: ''
    }
  },
  methods: {
    onLoadUser() {
      this.$router.push('/users/' + this.userId);
    }
  }
}
</script>
