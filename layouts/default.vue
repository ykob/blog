<template lang="pug">
  v-app
    v-app-bar(
      color = 'white'
      app
      elevation = '1'
      )
      v-toolbar-title
        |Blog
      v-spacer
      v-app-bar-nav-icon
    v-main.blue-grey.lighten-5
      v-container
        nuxt
    v-footer(
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
