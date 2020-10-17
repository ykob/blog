<template lang="pug">
v-footer(
  v-if = 'isShown'
  dark
  color = 'blue-grey'
  )
  v-btn(
    href = 'https://www.tplh.net/'
    target = '_blank'
    x-small
    height = '24'
    text
    )
    |Written by Yoichi Kobayashi
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
