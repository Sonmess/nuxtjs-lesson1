<template>
  <div class="container">
    <div>
      <Logo />
      <h1 class="title">
        lesson-1
      </h1>
      <Header></Header>

      <div class="links">
        <nuxt-link to="/users">Users</nuxt-link>
        <button @click="$router.push('/products')">Products</button>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "../components/Header";
export default {
  component: {
    Header: Header
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
