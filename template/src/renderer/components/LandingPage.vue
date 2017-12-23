<template>
  <ou-message-bar icon='Info'>
  Lorem ipsum dolor sit amet, a elit sem interdum consectetur adipiscing elit.
  <br />
  <ou-link @click="open">Go to Google.com</ou-link>
</ou-message-bar>
</template>

<script>
  export default {
    name: 'landing-page',
    methods: {
      open () {
        var link = 'http://www.google.com'
        this.$electron.shell.openExternal(link)
      }
    }
  }
</script>

<style>
</style>
