<template>
    <section class="footer-nav">
        <div class="container">
            <div class="navigations">
                <nav v-for="(el, index) in navLink" :key="`section-${index}`">
                    <h2>{{ el.title }}</h2>
                    <ul>
                        <li v-for="(link, index) in el.links" :key="`link-${index}`">
                            <a :href="link.url">{{ link.text }}</a>
                        </li>
                    </ul>
                </nav>
            </div>
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
    </section>
</template>

<script>
export default {
    name: 'FooterNav',
    data() {
        return {
            navLink: [
                {
                    title: 'DC comics',
                    links: [
                        {
                            text:'Characters',
                            url: '#',
                        },
                        {
                            text:'Comics',
                            url: '#',
                        },
                        {
                            text:'Movies',
                            url: '#',
                        },
                        {
                            text:'TV',
                            url: '#',
                        },
                        {
                            text:'Games',
                            url: '#',
                        },
                        {
                            text:'Videos',
                            url: '#',
                        },
                        {
                            text:'News',
                            url: '#',
                        }
                    ]
                },
                {
                    title: 'shop',
                    links: [
                        {
                            text:'Shop DC',
                            url: '#',
                        },
                        {
                            text:'Shop DC Collectibles',
                            url: '#',
                        }
                    ]
                },
                {
                    title: 'DC',
                    links: [
                        {
                            text:'Terms of use',
                            url: '#',
                        },
                        {
                            text:'Privacy policy (new)',
                            url: '#',
                        },
                        {
                            text:'Ad Choices',
                            url: '#',
                        },
                        {
                            text:'Advertising',
                            url: '#',
                        },
                        {
                            text:'Jobs',
                            url: '#',
                        },
                        {
                            text:'Subscriptions',
                            url: '#',
                        },
                        {
                            text:'Talent Workshops',
                            url: '#',
                        },
                        {
                            text:'CPSC Certificates',
                            url: '#',
                        },
                        {
                            text:'Ratings',
                            url: '#',
                        },
                        {
                            text:'Shop Help',
                            url: '#',
                        },
                        {
                            text:'Contact Us',
                            url: '#',
                        }
                    ]
                },
                {
                    title: 'sites',
                    links: [
                        {
                            text:'DC',
                            url: '#',
                        },
                        {
                            text:'MAD Magazine',
                            url: '#',
                        },
                        {
                            text:'DC Kids',
                            url: '#',
                        },
                        {
                            text:'DC Universe',
                            url: '#',
                        },
                        {
                            text:'DC Power Visa',
                            url: '#',
                        }
                    ]
                },
                
            ]
        }
    },
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

    .footer-nav {
        position: relative;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        height: 360px;
        z-index: -2;
        
        .container {
            position: relative;
            display: flex;
            justify-content: space-between;
            max-height: 100%;

            .navigations {
                display: flex;
                flex-direction: column;
                flex-wrap: wrap;
                width: calc(100% / 3);
                max-height: 100%;
                

                nav {
                    width: calc(100% / 3);
                    padding: 1rem;

                    h2 {
                        font-size: 1rem;
                        color: $light-col;
                        text-transform: uppercase;
                    }

                    ul {
                        list-style: none;

                        a {
                            font-size: 0.8rem;
                            text-decoration: none;
                            color: $dark-col;

                            &:hover {
                                color: $light-col;
                            }
                        }
                    }
                }
            }

            img {
                position: absolute;
                bottom: 0;
                right: 0;
                transform: translateY(15%);
                z-index: -1;
            }
        }
        
    }
</style>