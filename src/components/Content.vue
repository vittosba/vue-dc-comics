<template>
  <section>
      <div class="container">
          <ul>
              <li v-for="(el, index) in cards" :key="`card-${index}`">
                  <Card :url="el.thumb" :text="el.series"/>
              </li>
          </ul>

          <button>Load More</button>
      </div>
  </section>
</template>

<script>
import DcComics from '@/data/dc-comics.js'
import Card from '@/components/Card.vue'

export default {
    name: 'Content',
    components: {
        Card,
    },
    data() {
        return {
            cards: DcComics,
        }
    }
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

    section {
        background: #1c1c1c;
    }
    .container {
        padding: 2rem;
        text-align: center;

        ul {
            display: flex;
            flex-wrap: wrap;

            li {
                width: calc(100% / 6);
                padding: 1rem;
            }
        }

        button {
            background: $primary-col;
            padding: 1rem 3rem;
            border: none;
        }
    }
</style>