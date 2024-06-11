<script>
import AppMainBanner from './AppMainBanner.vue';
import AppMainWrapper from './AppMainWrapper.vue';
export default {
    components: {
        AppMainBanner,
        AppMainWrapper
    },
    data() {
        return {

        }
    }
}
</script>

<template>
    <main>
        <figure>
            <img src="../assets/img/jumbotron.jpg" alt="">
        </figure>
        <AppMainWrapper />
        <AppMainBanner />
    </main>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

main {
    background-color: $dc-black;
    color: white;
}

figure {
    height: 500px;
    width: 100%;
    overflow: hidden;
    img {
        width: 100%;
    }
    }
</style>