<template>
  <section>
      <div class="container">
        <h2>Content goes here</h2>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Content',
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

    section {
        background: #000;
    }
    .container {
        padding: 2rem;

        h2 {
            color: $light-col;
        }
    }
</style>