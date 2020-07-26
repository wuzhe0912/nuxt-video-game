<template lang="pug">
  .navigation__wrap
    nuxt-link.navigation__list(v-for="node in list" :to="node.link") {{ node.name }}
</template>

<script>
export default {
  data () {
    return {
      list: [
        { name: 'Home', link: '/' },
        { name: 'About', link: '/about' }
      ]
    }
  }
}
</script>

<style lang="scss">

</style>
