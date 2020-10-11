<template lang="pug">
  v-app
    AppBar
    NavigationDrawer
    v-main.blue-grey.lighten-5
      nuxt
    Footer
</template>

<script>
import AppBar from '@/components/AppBar'
import Footer from '@/components/Footer'
import NavigationDrawer from '@/components/NavigationDrawer'

export default {
  components: {
    AppBar,
    Footer,
    NavigationDrawer,
  },
}
</script>
