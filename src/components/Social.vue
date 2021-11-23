<template>
  <section class="social">
      <div class="container">
          <button>Sign-up now!</button>
          <ul>
              <li>Follow us</li>
              <li><img src="../assets/img/footer-facebook.png" alt=""></li>
              <li><img src="../assets/img/footer-twitter.png" alt=""></li>
              <li><img src="../assets/img/footer-youtube.png" alt=""></li>
              <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
              <li><img src="../assets/img/footer-periscope.png" alt=""></li>
          </ul>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Social',
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

    .social {
        background: #303030;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 2rem;

            button {
                color: $light-col;
                background: #303030;
                padding: 0.8rem;
                text-transform: uppercase;
                border: 1px solid $primary-col;
            }

            ul {
                display: flex;
                align-items: center;
                list-style: none;
                
                li {
                    margin-right: 1rem;
                    &:first-child {
                        color: $primary-col;
                        text-transform: uppercase;
                    }
                }
            }
        }
    }
</style>