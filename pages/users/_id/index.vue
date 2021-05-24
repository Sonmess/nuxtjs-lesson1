<template>
  <h1>Hi single user with ID: {{$route.params.id}}</h1>
</template>

<script>
export default {
  name: "index",
  validate(data) {
    return /^\d+$/.test(data.params.id);
  }
}
</script>
