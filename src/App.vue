<template>

  <div id="app">

    <Nav />

    <div class="container">

      <router-view />

    </div>

    <Footer />

  </div>

</template>

<script>

import Nav from '@/components/Nav'
import Footer from '@/components/Footer'
import {
  setDocumentDirectionPerLocale,
  setDocumentLang,
  setDocumentTitle
} from '@/util/i18n/document'

export default {
  name: 'App',
  components: { Nav, Footer },
  mounted () {
    this.$watch(
      '$i18n.locale',
      (newLocale, oldLocale) => {
        if (newLocale === oldLocale) {
          return
        }
        setDocumentLang(newLocale)
        setDocumentDirectionPerLocale(newLocale)
        setDocumentTitle(this.$t('app.title'))
      },
      { immediate: true }
    )
  }
}

</script>

<style>

body {

  margin: 0;

}

#app {

  font-family: "Avenir", Helvetica, Arial, sans-serif;

  -webkit-font-smoothing: antialiased;

  -moz-osx-font-smoothing: grayscale;

  color: #2c3e50;

}

#app .container {

  padding: 1rem;

}

</style>
