<template>
  <div style="padding: 50px">
    <h1> Welcome! </h1>
    <br>
    <br>
    <nuxt-link to="/es/">ES/</nuxt-link>
    <br>
    <br>
    <span>Current route:  </span>{{ $router.currentRoute.fullPath }}
    <br>
    <br>
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>
