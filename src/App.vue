<template>
  <div id="app">
    <Header />
    <Hero />
    <main>
      <Content />
    </main>

    <footer>
      <FooterNav />

      <Social />
    </footer>
  </div>
</template>

<script>

import Header from '@/components/Header.vue'
import Content from '@/components/Content.vue'
import FooterNav from '@/components/FooterNav.vue'
import Social from '@/components/Social.vue'
import Hero from '@/components/Hero.vue'

export default {
  name: 'App',
  components: {
    Header,
    Content,
    FooterNav,
    Social,
    Hero,
  }
}
</script>

<style lang="scss">
@import '@/styles/globals';
@import '@/styles/utilities';
</style>
