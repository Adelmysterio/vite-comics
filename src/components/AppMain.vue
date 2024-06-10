<script>
import AppMainJumbo from './AppMainJumbo.vue';
export default {
    components: {
        AppMainJumbo
    },
    data() {
        return {

        }
    }
}
</script>

<template>
    <main>
        <div class="container">
            <h2> Content goes here </h2>
        </div>
        <AppMainJumbo />
    </main>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

main {
    background-color: $dc-black;
    color: white;

    h2 {
        padding: 4rem 0;
    }
}
</style>