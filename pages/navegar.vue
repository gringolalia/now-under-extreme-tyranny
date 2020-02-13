<template lang="pug">
section.container
  .md-layout.md-gutter.md-alignment-top-center
    .md-layout-item.md-medium-size-50.md-small-size-100
      img(src="/biohazard.svg" width='100px')
      h1.dignity.mb-5(style="margin: 15px 15px")
        | &nbsp; Navegar é Impreciso
      h3.dignity(style="margin-bottom: 15px")
        | These Are the Fruits of Nuxt
      md-button.md-raised.md-primary(style="margin-bottom: 25px")
        i.material-icons wb_sunny
        | &nbsp; Going Nuxt

    .md-layout-item.md-medium-size-50.md-small-size-100
      img(src="/biohazard.svg" width='100px')
      h1.dignity(style="margin: 15px 15px")
        | &nbsp; Navegar é Impreciso
      h3.dignity(style="margin-bottom: 15px")
        | The Nuxt Best Thing to Being There
      md-button.md-accent.md-raised(@click='showDialog = true')
        i.material-icons wb_sunny
        | &nbsp; Nuxt and Bolts

    .md-layout-item.md-medium-size-50.md-small-size-100
      img(src="/biohazard.svg" width='100px')
      h1.dignity(style="margin: 15px 15px")
        | &nbsp; Navegar é Impreciso
      h3.dignity(style="margin-bottom: 15px")
        | The Nuxt Big Thing
      md-button.md-accent.md-raised(@click='showDialog = true')
        i.material-icons wb_sunny
        | &nbsp; Nuxt To You

    .md-layout-item.md-medium-size-50.md-small-size-100
      img(src="/biohazard.svg" width='100px')
      h1.dignity(style="margin: 15px 15px")
        | &nbsp; Navegar é Impreciso
      h3.dignity(style="margin-bottom: 15px")
        | Getting Nuxt To You
      md-button.md-accent.md-raised(@click='showDialog = true')
        i.material-icons wb_sunny
        | &nbsp; Nuxt in a Tux

    md-dialog(:md-active.sync='showDialog' style="width: 350px")
      md-dialog-title(style="padding: 15px; color:white; background-color: #607d8b")
        i.fa.fa-gears.fa-2x
        | &nbsp; The New Market Machines
      md-content
        blockquote.dignity(style="line-height: 150%; font-size:16px") All truth passes through three stages. First, it is ridiculed. Second, it is violently opposed. Third, it is accepted as being self-evident.
        p(style="text-align:center; padding-top: 12px;") &mdash; Schopenhauer

      md-dialog-actions
        md-button.md-primary.md-raised(@click='showDialog = false')
          md-icon expand_more
          | &nbsp;Depress

        md-button.md-accent.md-raised(@click='showDialog = false')
          md-icon expand_less
          | &nbsp; Impress
</template>

<script>
  export default {
    name: 'DialogCustom',
    data: () => ({
      showDialog: false
    })
  }
</script>


<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

  .md-dialog {
    max-width: 768px;
  }

.title {
  font-family: "News Cycle", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
