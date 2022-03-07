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
import 'boxicons'

Vue.use(VueI18n) // Internationalization
Vue.use(Vuesax, {
  colors: {
      primary:'#005f73',
      success:'#fff',
      danger:'rgb(242, 19, 93)',
      warning:'#94d2bd',
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
