<template lang="pug">
  v-app
    v-app-bar(
      dark
      color = 'blue-grey darken-3'
      app
      elevation
      )
      v-toolbar-title
        |Blog
      v-spacer
      v-app-bar-nav-icon
    v-main
      v-container
        nuxt
    v-footer(
      color = 'blue-grey lighten-5'
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
