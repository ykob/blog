<template lang="pug">
div
  v-row(
    dense
    )
    v-col(
      :cols = '12'
      :md = '4'
      :sm = '6'
      )
      h1.text-h1.mb-4
        |Blog
      p
        |フロントエンド開発に関する覚書
      .d-flex.align-center
        .mr-2
          |Yoichi Kobayashi
        v-btn(
          icon
          href = 'https://github.com/ykob'
          )
          v-icon
            |mdi-github
        v-btn(
          icon
          href = 'https://twitter.com/ykob0123'
          )
          v-icon
            |mdi-twitter
        
    v-col(
      :cols = '12'
      :md = '4'
      :sm = '6'
      )
      v-card
        v-img(
          class = 'align-end'
          height = '200px'
          )
          v-card-title
            |Article Title
        v-card-subtitle(
          class = 'pb-0'
          )
          |Oct 1, 2020
        v-card-text(
          class = 'text--primary'
          )
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
