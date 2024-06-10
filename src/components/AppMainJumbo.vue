<script>
import digitalComicsImage from '../assets/img/buy-comics-digital-comics.png';
import dcMerchandiseImage from '../assets/img/buy-comics-merchandise.png';
import subscriptionImage from '../assets/img/buy-comics-subscriptions.png';
import comicShopLocatorImage from '../assets/img/buy-comics-shop-locator.png';
import dcPowerVisaImage from '../assets/img/buy-dc-power-visa.svg';

export default {
    data() {
        return {
            Jumbolist: [
                {
                    name: 'DIGITAL COMICS',
                    image: digitalComicsImage
                },
                {
                    name: 'DC MERCHANDISE',
                    image: dcMerchandiseImage
                },
                {
                    name: 'SUBSCRIPTION',
                    image: subscriptionImage
                },
                {
                    name: 'COMIC SHOP LOCATOR',
                    image: comicShopLocatorImage
                },
                {
                    name: 'DC POWER VISA',
                    image: dcPowerVisaImage
                },
            ]
        }
    }
}
</script>

<template>
    <div class="jumbo">
        <ul>
            <li v-for="(item, index) in Jumbolist" :key="index">
                <figure>
                    <img :src="item.image" alt="">
                </figure>
                <a href="#">
                    {{ item.name }}
                </a>
            </li>
        </ul>
    </div>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

.jumbo {
    background-color: $dc-blue;
    display: flex;
    justify-content: center;
}

a {
    text-decoration: none;
    color: white;
    font-size: 1rem;
    font-weight: normal;
}

ul {
    display: flex;
    justify-content: space-evenly;
    max-width: 1200px;
    width: 100%;
    padding: 4rem 0;
}

li {
    display: flex;
    align-items: center;
}

li:last-child figure {
    height: 2rem;
    margin-right: 1rem;
}

figure {
    height: 3rem;
    width: 3rem;

}

img {
    height: 100%;
}

</style>