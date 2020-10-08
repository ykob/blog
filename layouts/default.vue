<template lang="pug">
  v-app
    AppBar
    v-navigation-drawer(
      app
      )
      .text-h1
        |Blog
      v-divider
      v-list
        v-list-item
          |Menu
        v-list-item
          |Menu
    v-main.blue-grey.lighten-5
      nuxt
    Footer
</template>

<script>
import AppBar from '@/components/AppBar'
import Footer from '@/components/Footer'

export default {
  components: {
    AppBar,
    Footer,
  },
}
</script>
