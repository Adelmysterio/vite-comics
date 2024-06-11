<script>
import AppFooterJumbo from './AppFooterJumbo.vue';
export default {
    components: { 
        AppFooterJumbo 
    },

    data() {
        return {
            comicsLinks: [
                {
                    name: "Characters",
                    url: '#',
                    active: false
                },
                {
                    name: "Comics",
                    url: '#',
                    active: false
                },
                {
                    name: "Movies",
                    url: '#',
                    active: false
                },
                {
                    name: "Tv",
                    url: '#',
                    active: false
                },
                {
                    name: "Games",
                    url: '#',
                    active: false
                },
                {
                    name: "Videos",
                    url: '#',
                    active: false
                },
                {
                    name: "News",
                    url: '#',
                    active: false
                },
            ],
            shopLinks: [
                {
                    name: "Shop DC",
                    url: '#',
                    active: false
                },
                {
                    name: "Shop DC Collectibles",
                    url: '#',
                    active: false
                },
            ],
            dcLinks: [
                {
                    name: "Terms of Use",
                    url: '#',
                    active: false
                },
                {
                    name: "Privacy policy (New)",
                    url: '#',
                    active: false
                },
                {
                    name: "Ad Choices",
                    url: '#',
                    active: false
                },
                {
                    name: "Advertising",
                    url: '#',
                    active: false
                },
                {
                    name: "Jobs",
                    url: '#',
                    active: false
                },
                {
                    name: "Subscriptions",
                    url: '#',
                    active: false
                },
                {
                    name: "Talent Workshops",
                    url: '#',
                    active: false
                },
                {
                    name: "CPSC Certificates",
                    url: '#',
                    active: false
                },
                {
                    name: "Ratings",
                    url: '#',
                    active: false
                },
                {
                    name: "Shop Help",
                    url: '#',
                    active: false
                },
                {
                    name: "Contact Us",
                    url: '#',
                    active: false
                },
            ],
            sitesLinks: [

                {
                    name: "DC",
                    url: '#',
                    active: false
                },
                {
                    name: "MAD Magazine",
                    url: '#',
                    active: false
                },
                {
                    name: "DC Kids",
                    url: '#',
                    active: false
                },
                {
                    name: "DC Universe",
                    url: '#',
                    active: false
                },
                {
                    name: "DC Power Visa",
                    url: '#',
                    active: false
                },
            ]
        }
    }
}
</script>

<template>
    <footer>
        <div class="container">
            <nav>
                <section>
                    <h3>dc comics</h3>
                    <ul class="mb-1">
                        <li v-for="(item, index) in comicsLinks" :key="index"><a href="">{{ item.name }}</a></li>
                    </ul>
                    <h3>shop</h3>
                    <ul>
                        <li v-for="(item, index) in shopLinks" :key="index"><a href="">{{ item.name }}</a></li>
                    </ul>
                </section>
                <section>
                    <h3>dc</h3>
                    <ul>
                        <li v-for="(item, index) in dcLinks" :key="index"><a href="">{{ item.name }}</a></li>
                    </ul>
                </section>
                <section>
                    <h3>sites</h3>
                    <ul>
                        <li v-for="(item, index) in sitesLinks" :key="index"><a href="">{{ item.name }}</a></li>
                    </ul>
                </section>
            </nav>
            <figure>
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </figure>
        </div>
        <AppFooterJumbo />
    </footer>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

footer {
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 25rem;
    

    div {
        justify-content: space-between;
        display: flex;


        nav {
            display: flex;
            margin: 3rem 0;
            width: 60%;
            
            section {
                margin-right: 3rem;
            }
        }

        figure {
            position: relative;
            width: 70%;
            overflow: hidden;

            img {
                position: absolute;
                right: 0;
                top: -100px
            }
        }
    }


}

a {
    text-decoration: none;
    color: $dc-lightgray;
}

h3 {
    font-size: 1.2rem;
    color: white;
    text-transform: uppercase;
    margin-bottom: 1rem;
}

li {
    margin-bottom: .4rem;
}
</style>