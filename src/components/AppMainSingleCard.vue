<script>
export default {
    data() {
        return {

        }
    },

    props: {
        img: String,
        comicTitle: String
    }
}
</script>

<template>
    <article>
        <figure>
            <img :src="img" :alt="comicTitle">
        </figure>
        <h4>{{ comicTitle }}</h4>
    </article>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

article {
    width: calc(100% / 6 - 2rem);
    height: 200px;
    margin: 1rem;
    margin-bottom: 4rem;

    figure {
        width: 100%;
        height: 100%;
        overflow: hidden;
        margin-bottom: 1rem;

        img {
            width: 100%;
        }

    }

    h4 {
        text-transform: uppercase;
    }
}
</style>