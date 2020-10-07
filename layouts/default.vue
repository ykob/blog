<template lang="pug">
  v-app
    v-app-bar(
      color = 'white'
      app
      elevation = '1'
      )
      v-sheet
        v-toolbar-title
          |Blog
      v-spacer
      v-app-bar-nav-icon
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
      v-container
        nuxt
    v-footer(
      app
      dark
      color = 'blue-grey'
      )
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
</template>

<script>
export default {}
</script>
