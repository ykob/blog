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
        v-list-item(
          link
          )
          v-list-item-icon
            v-icon
              |mdi-home
          v-list-item-title
            |Home
        v-list-group(
          no-action
          )
          template(
            v-slot:activator
            )
            v-list-item-icon
              v-icon
                |mdi-home
            v-list-item-title
              |Categories
          v-list-item(
            link
            )
            v-list-item-title
              |Menu
      v-divider
      v-sheet
        v-btn(
          icon
          href = 'https://github.com/ykob'
          target = '_blank'
          )
          v-icon
            |mdi-github
        v-btn(
          icon
          href = 'https://twitter.com/ykob0123'
          target = '_blank'
          )
          v-icon
            |mdi-twitter
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
