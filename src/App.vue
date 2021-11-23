<template>
  <div id="app">
    <Header />

    <main>
      <Content />
    </main>

    <footer>
      <FooterNav />
    </footer>
  </div>
</template>

<script>

import Header from '@/components/Header.vue'
import Content from '@/components/Content.vue'
import FooterNav from '@/components/FooterNav.vue'

export default {
  name: 'App',
  components: {
    Header,
    Content,
    FooterNav,
  }
}
</script>

<style lang="scss">
@import '@/styles/globals';
@import '@/styles/utilities';
</style>
