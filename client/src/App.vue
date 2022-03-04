<template>
  <div id="q-app">
    <router-view />
  </div>
</template>
<script>
import Vue from 'vue'
import VueI18n from 'vue-i18n'
import Vuesax from 'vuesax'
import 'vuesax/dist/vuesax.css'

Vue.use(VueI18n) // Internationalization
Vue.use(Vuesax, {
  colors: {
      primary:'#1976D2',
      success:'#26A69A',
      danger:'rgb(242, 19, 93)',
      warning:'rgb(255, 130, 0)',
      dark:'rgb(36, 33, 69)'
    }
})
const messages = {
  es: {},
  en: {}
}
export const i18n = new VueI18n({
  locale: 'es',
  fallbackLocale: 'en',
  messages
})

export default {
  name: 'App'
}
</script>
