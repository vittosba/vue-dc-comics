<template>
  <header>
      <div class="container">
          <a href="#">
              <img src="../assets/img/dc-logo.png" alt="">
          </a>
          <nav>
              <ul>
                  <li v-for="(link, index) in navLink" :key="`link-${index}`">
                      <a :class="{active: link.current}" :href="link.url">{{ link.text }}</a>
                  </li>
              </ul>
          </nav>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            navLink: [
                {
                    text: 'characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'tv',
                    url: '#',
                    current: false,
                },
                {
                    text: 'games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'news',
                    url: '#',
                    current: false,
                },
                {
                    text: 'shop',
                    url: '#',
                    current: false,
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

    header {
        background: $light-col;
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem;
    
            nav {
                ul {
                    display: flex;
                    list-style: none;
                    
                    a {
                        font-size: 0.9rem;
                        display: inline-block;
                        margin: 0 1rem;
                        padding: 1rem 0;
                        text-decoration: none;
                        color: $dark-col;
                        text-transform: uppercase;
                        &.active,
                        &:hover {
                            color: $primary-col;
                            border-bottom: 3px solid $primary-col;
                        }
                    }
                }
            }
        }
    }
</style>