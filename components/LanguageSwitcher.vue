<template>
  <div>
    <p>Lang Switcher</p>
    <br>
    <nuxt-link
      v-for="locale in availableLocales"
      :key="locale.code"
      :to="switchLocalePath(locale.code)">{{ locale.name }}
    </nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'LangSwitcher',
  computed: {
    availableLocales () {
      return this.$i18n.locales.filter(i => i.code !== this.$i18n.locale)
    }
  }
}
</script>

<style>
.nuxt-logo {
  height: 180px;
}
</style>
