
<template>
  <div id="app">
    <AppNavbar/>
    <router-view/>
    <Notification/>
  </div>
</template>

<script>
import AppNavbar from './containers/app_navbar'
import Notification from './containers/app_notification'

export default {
  name: 'app',

  // Top-Level Application Components
  components: {
    AppNavbar,
    Notification
  },

  // Top-Level page Meta
  metaInfo: {
    title: 'Loading...', // set a title
    titleTemplate: 'HotSheets - %s', // title is now "HotSheets - Loading..."
    htmlAttrs: {
      lang: 'en'
    }
  }

}
</script>

<style lang="sass">
  @import "./sass/vendor.sass"

  html
    height: 100%

  body
    height: 100%

  .container-fluid
    height: 100%

  #app
    height: 100%

</style>
