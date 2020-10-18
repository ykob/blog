<template lang="pug">
v-app-bar(
  v-if = 'isShown'
  color = 'white'
  app
  elevation = '1'
  )
  v-sheet
    v-toolbar-title
      |Blog
  v-spacer
  v-app-bar-nav-icon(
    @click = '$store.commit("toggleDrawer")'
    )
</template>

<script>
export default {
  computed: {
    isShown() {
      switch (this.$vuetify.breakpoint.name) {
        case 'xs':
        case 'sm':
        case 'md':
          return true
        case 'lg':
        case 'xl':
        default:
          return false
      }
    },
  },
}
</script>
