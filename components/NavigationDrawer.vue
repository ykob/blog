<template lang="pug">
v-navigation-drawer(
  app
  color = 'blue-grey'
  )
  v-sheet
    .text-h1.px-3.pt-2.pb-6
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
              |mdi-label
          v-list-item-title
            |Categories
        v-list-item(
          link
          )
          v-list-item-title
            |Menu
      v-list-item
        v-text-field(
          label = '記事検索'
          append-icon = 'mdi-magnify'
          )
  v-sheet.pa-4(
    dark
    color = 'transparent'
    )
    p
      |yoichi kobayashi
    v-btn(
      icon
      href = 'https://github.com/ykob'
      target = '_blank'
      )
      v-icon(
        color = 'white'
        )
        |mdi-github
    v-btn(
      icon
      href = 'https://twitter.com/ykob0123'
      target = '_blank'
      )
      v-icon(
        color = 'white'
        )
        |mdi-twitter
</template>

<script>
export default {}
</script>
