<template>
  <div style="padding: 50px">
    <h1> Welcome! </h1>
    <br>
    <br>
    <br>
    <NuxtLink to="/">Home page</NuxtLink>
    <br>
    <NuxtLink to="/products">Products page</NuxtLink>
    <br>
    <br>
    <span>Current route:  </span>{{ $router.currentRoute.fullPath }}
    <br>
    <br>
    <language-switcher></language-switcher>
  </div>
</template>

<script>
import languageSwitcher from '../components/LanguageSwitcher.vue';

export default {
  components:{
    languageSwitcher,
  },
  name: 'IndexPage'
}
</script>
