<template>
  <div class="card">
      <img :src="url" :alt="text">
      <div class="text">{{text}}</div>
  </div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        url: String, // Number, Boolean, Object, Array..
        text: String,
    }
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

    .card {
        .text {
            color: $light-col;
        }
    }
</style>