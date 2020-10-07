<template lang="pug">
div
  v-row(
    dense
    )
    v-col(
      v-for = 'item, i in items'
      :key = 'i'
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
  data: () => ({
    items: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
  }),
}
</script>
