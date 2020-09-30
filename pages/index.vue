<template lang="pug">
div
  h1
    |Blog
  v-row(
    dense
    )
    v-col(
      :cols = '12'
      :md = '4'
      :sm = '6'
      )
      v-card
        v-card-title
          |Article Title
        v-card-text
          |article description text text
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo,
  },
}
</script>
